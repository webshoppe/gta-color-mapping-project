# 📄 How to Properly Import CSVs and Preserve Leading Zeros

Some columns (like “Crew Code(s)”) contain values such as `00`.  
To ensure these codes display correctly (and not as `0`), you must import the CSV using the steps below.

## Excel: Import Wizard Steps

1. **Open Excel** (do NOT double-click the CSV).
2. Go to **Data > Get Data > From File > From Text/CSV** (or just **Data > From Text/CSV**).
3. Select your CSV file and click **Import**.
4. In the import dialog, click **Transform Data** or "Advanced Options".
5. Find the "Crew Code(s)" column in the preview.
6. Set its data type to **Text**.
7. Finish import.

*Older Excel:*  
- Enable legacy import wizards in File > Options > Data.
- Use **Data > Get Data > Legacy Wizards > From Text** and set the column type to Text in Step 3.

## LibreOffice Calc: Text Import Steps

1. **Open LibreOffice Calc**.
2. Go to **File > Open** and select your CSV.
3. In the **Text Import** dialog, find the “Crew Code(s)” column.
4. Click the column header and set the column type to **Text**.
5. Click **OK**.

## Google Sheets

1. Go to **File > Import > Upload** and select your CSV.
2. In import options, set “Convert text to numbers, dates, and formulas” to **No**.
3. Complete the import.

> **Tip:**  
> If you double-click a CSV, Excel or LibreOffice may strip leading zeros. Always use the import wizard!

## 🏷️ About “Flattened” Headers

- In the original Excel files, some columns have headers with line breaks for readability (e.g.,  

Color
Effect/Family

).
- In the CSVs, these headers are “flattened” for compatibility:
- **Example:**  
  - Excel: `Color\nEffect/Family`  
  - CSV: `Color / Effect/Family`
- This ensures all columns have a single, clear header row and are easy to use in scripts and data tools.

## 🛠️ Macro/Template Option: Forcing Text Columns in Excel

If you want to make things even easier for your users, you can provide an **Excel macro-enabled template** (`.xlsm`) or a pre-formatted `.xlsx` with the "Crew Code(s)" column already set to Text:

**How to Create a Template:**

1. Open your `.xlsx` in Excel.
2. Select the "Crew Code(s)" column.
3. Right-click > **Format Cells** > set to **Text**.
4. Save as `.xltx` (Excel Template) or `.xlsm` (if you want to include a macro).

**Optional Macro to Force Text Format on Open:**  
Place this in `ThisWorkbook` in the VBA editor.

<pre>```Private Sub Workbook_Open()
Sheets("Livery").Columns("D:D").NumberFormat = "@"
End Sub```</pre>

- This macro will set column D (adjust as needed) to Text every time the workbook is opened.

## 📚 Quick Reference Table

| File Type    | Leading Zeros Preserved by Default? | User Action Needed? | Notes                                 |
|--------------|-------------------------------------|---------------------|---------------------------------------|
| .csv         | No                                  | Yes (import wizard) | Use steps above for Excel/LO/Sheets   |
| .xlsx        | Yes                                 | No                  | Use as master for sharing             |
| .ods         | Yes                                 | No                  | Use for LibreOffice                   |
| .xltx/.xlsm  | Yes (if formatted)                  | No                  | Use template for repeated imports     |

---

**If you see `00` turn into `0`, re-import using the steps above!**
