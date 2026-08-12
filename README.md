# Power BI Model Export

[![Link Check](https://github.com/hihipy/pbi-model-export/actions/workflows/links.yml/badge.svg)](https://github.com/hihipy/pbi-model-export/actions/workflows/links.yml)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

**Built with**

[![C#](https://img.shields.io/badge/C%23-512BD4?style=flat&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMS4xOTQgNy41NDN2OC45MTNjMCAxLjEwMy41ODggMi4xMjIgMS41NDQgMi42NzRsNy43MTggNC40NTZhMy4wODYgMy4wODYgMCAwIDAgMy4wODggMGw3LjcxOC00LjQ1NmEzLjA4NyAzLjA4NyAwIDAgMCAxLjU0NC0yLjY3NFY3LjU0M2EzLjA4NCAzLjA4NCAwIDAgMC0xLjU0NC0yLjY3M0wxMy41NDQuNDE0YTMuMDg2IDMuMDg2IDAgMCAwLTMuMDg4IDBMMi43MzggNC44N2EzLjA4NSAzLjA4NSAwIDAgMC0xLjU0NCAyLjY3M1ptNS40MDMgMi45MTR2My4wODdhLjc3Ljc3IDAgMCAwIC43NzIuNzcyLjc3My43NzMgMCAwIDAgLjc3Mi0uNzcyLjc3My43NzMgMCAwIDEgMS4zMTctLjU0Ni43NzUuNzc1IDAgMCAxIC4yMjYuNTQ2IDIuMzE0IDIuMzE0IDAgMSAxLTQuNjMxIDB2LTMuMDg3YzAtLjYxNS4yNDQtMS4yMDMuNjc5LTEuNjM3YTIuMzEyIDIuMzEyIDAgMCAxIDMuMjc0IDBjLjQzNC40MzQuNjc4IDEuMDIzLjY3OCAxLjYzN2EuNzY5Ljc2OSAwIDAgMS0uMjI2LjU0NS43NjcuNzY3IDAgMCAxLTEuMDkxIDAgLjc3Ljc3IDAgMCAxLS4yMjYtLjU0NS43Ny43NyAwIDAgMC0uNzcyLS43NzIuNzcxLjc3MSAwIDAgMC0uNzcyLjc3MlptMTIuMzUgMy4wODdhLjc3Ljc3IDAgMCAxLS43NzIuNzcyaC0uNzcydi43NzJhLjc3My43NzMgMCAwIDEtMS41NDQgMHYtLjc3MmgtMS41NDR2Ljc3MmEuNzczLjc3MyAwIDAgMS0xLjMxNy41NDYuNzc1Ljc3NSAwIDAgMS0uMjI2LS41NDZ2LS43NzJIMTJhLjc3MS43NzEgMCAxIDEgMC0xLjU0NGguNzcydi0xLjU0M0gxMmEuNzcuNzcgMCAxIDEgMC0xLjU0NGguNzcydi0uNzcyYS43NzMuNzczIDAgMCAxIDEuMzE3LS41NDYuNzc1Ljc3NSAwIDAgMSAuMjI2LjU0NnYuNzcyaDEuNTQ0di0uNzcyYS43NzMuNzczIDAgMCAxIDEuNTQ0IDB2Ljc3MmguNzcyYS43NzIuNzcyIDAgMCAxIDAgMS41NDRoLS43NzJ2MS41NDNoLjc3MmEuNzc2Ljc3NiAwIDAgMSAuNzcyLjc3MlptLTMuMDg4LTIuMzE1aC0xLjU0NHYxLjU0M2gxLjU0NHYtMS41NDNaIi8%2BPC9zdmc%2B)](https://learn.microsoft.com/en-us/dotnet/csharp/)
[![DAX](https://img.shields.io/badge/DAX-CF8B0E?style=flat&logoColor=black)](https://learn.microsoft.com/en-us/dax/)
[![Power BI](https://img.shields.io/badge/Power%20BI-CF8B0E?style=flat&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyBmaWxsPSIjMDAwMDAwIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMTAgMTJhMSAxIDAgMCAxIDEgMXYxMUg0YTEgMSAwIDAgMS0xLTFWMTNhMSAxIDAgMCAxIDEtMWg2Wm0tMi0uNVY3YTEgMSAwIDAgMSAxLTFoNmExIDEgMCAwIDEgMSAxdjE3aC00LjVWMTNhMS41IDEuNSAwIDAgMC0xLjUtMS41SDhabTUtNlYxYTEgMSAwIDAgMSAxLTFoNmExIDEgMCAwIDEgMSAxdjIyYTEgMSAwIDAgMS0xIDFoLTMuNVY3QTEuNSAxLjUgMCAwIDAgMTUgNS41aC0yWiIvPjwvc3ZnPg%3D%3D)](https://powerbi.microsoft.com)
[![Tabular Editor 2](https://img.shields.io/badge/Tabular%20Editor%202-007060?style=flat&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAESklEQVR4nO2bP4%2FcRBiHn9e7uaSgRugUXRB%2FEkAoBUKQ7qTkIhREQcnnoKKioKDjOyC%2BBKAkSCkQDRJSikSQCJF%2F16QEIbjs%2Bkcx4%2BzGrD2z67E39vmRrN3T2ePxs69n3hmPTZLoPzlgwO%2FARTO7L2liZvOmBWeNq%2FZ8kAECXgW%2BlXTazOaSJikKHgoZMAfeAq6nkjQkQQATYAacBa6lkDQ0QQBTnKRzJIikIQqChaTGkTRUQfBsJG0saciCIIEkWyMPynFdad8wnKQd4DZwYGaHsXnSOoKGwiGwb2Z3YyRNIwrMcbfi58DP%2FnveuJrbIQdOABckmZndCUpSmJn%2F3O%2FsMlpG0keS7kna9X9XtkkxEVTwgi9ogstY%2B0hR9yNgD5cnXTazh1WRtI6g3PcApBgEboOi7v6HzoE3cL3bQZWkoXfzdWTAvwRSgOMsCCLypOMuCAKSRkGOSknrNNJRSMpILz43s7Zzr%2FIswEUze5RckL%2BQ5BcjKetQ0lngqqQPkwkqLkDSO8A%2Biwy8CUUZ35nZ7VTzzAGmuFzpTeBGyggqhiAfAF8mLBfgM5%2FQ3ZQ0NbNZ4vLLFHnSXhuN9N%2B4MP3HfzbdjoAXcSF%2F3sxmkpI3DSvIgLyNE2UsMvRU5c9ZSOoykrK%2BdPPFGKrzSOqLINiSpD4Jgi1I6psg6FhSG4KE6yJjtljKxxnwBCfpe0lve0mNHzWXaUPQCV%2Fujv%2Bs22JZdewJ%2F7%2BXgB8lvefHT0mvKWVYFpP%2Fj4HfcLdB3S96EjgTWfY93NzNKua%2BrK8kfQIc%2BvnmJA8jkgkqhgBm9rWkb2p2LTLu88AvkcV%2FDNxcOrZA7pSWS9rx35M%2BpWmlYasbVMr9vJK0VhvkJWiFAPlzHm1S1xCtCJJkNf%2FOvJy6fcqYLzOrE5s6eqC9CKqs6FIErV1mRQS1Sh%2FzoE4ZBQUYBQUYBQUYBQUYBQUYBQUYBQUYBQUYBQUYBQUYBQUYBQUYBQUYBQWYkmaRwSYI92g5dt%2BtMGUxjdm1pCnx81FdPIuvPPF93JLY0CR7KopoeAB8GnnMg9Kx3SHpZUm3%2FGLxJzULya%2F4%2FbuQ2ApF3SVdKV1bJZmZ%2FQFcxj2qKVZYdVFZkzSN3NaZv05K5ldtPQIuAb%2FSkSQzk5nNIretNdJZsZrTzB4CB3QoqQ9kAKOkap527aOk1TyT%2B1RIOkl%2F3w9rzP8SsGVJkg6Aq7i3Yorl%2BZN1H%2Fo9RxR1j06KV2aoJUmXgJ%2BAHb9AoZevQnnmAJL%2Bij2gNr%2FwkuaSXgfeB%2F7ELe%2Ft6yC3GFa9C3xBxBArmIAtSXoNuAHsJqhob4jKUJck7QLXcMv0j3C3aB8bJCPyLohO4ZckncZJOodLAbY20u6C6LbkuOZJazW2x1HSRqPk0u12Hfd%2B1SBvt42661IkdToL0DWN5lkqIqmrmclOaJTwrYikWyxeRhsESWbqliJpD%2FgBeAWXH%2FU1437Kf06QGr8B1Qz2AAAAAElFTkSuQmCC)](https://tabulareditor.com)

A Tabular Editor 2 C# script that exports a complete Power BI model to a structured JSON file built for AI consumption. It includes tables, columns, measures with full recursive DAX dependency chains, relationships with fact/dimension role hints, hierarchies, partitions, RLS roles, a compact summary section with top-level KPI detection, and a **data head** (first N rows sampled directly from source files on disk).

---

## Why

Power BI models contain structure that's invisible outside of Power BI Desktop. This script extracts everything into a single portable JSON file so you can:

- Give an AI assistant (Claude, Copilot, etc.) full context on your model, schema and actual data, without describing it manually
- Document model architecture for handoffs and reviews
- Run impact analysis on DAX measure dependencies
- Audit relationships, RLS roles, and data sources
- Compare models over time by diffing exports

---

## Requirements

- **Tabular Editor 2** (tested on 2.27; should work on any 2.x with C# scripting)
- **Power BI Desktop** model open in Tabular Editor (or SSAS/AAS connection)
- Source data files accessible on disk (local or OneDrive synced)

---

## Installation

1. Download `PBIModelExport.csx`
2. Open your Power BI model in Tabular Editor 2
3. Go to the **Advanced Scripting** tab
4. **File → Open Script** → select the `.csx` file
5. Click **Run** (▶)
6. Find the export in your Downloads folder, named automatically after your report

**Optional: save as a Custom Action:**

- **File → Preferences → Custom Actions**
- Click **Add**, paste the script contents
- Name it "Export Full Model to JSON"
- Now available via right-click context menu on any model

---

## Configuration

All options are at the top of the script:

```csharp
var headRowCount            = 50;    // rows to sample per table
var includeHiddenObjects    = true;  // include hidden tables/columns/measures
var includePartitionSources = true;  // include M queries and DAX partition expressions
var includeRoles            = true;  // include RLS role definitions

var outputFolder = Path.Combine(
    Environment.GetFolderPath(Environment.SpecialFolder.UserProfile), "Downloads");
```

The output file name is generated automatically from the report name, so there's no manual naming. If you have `Sales Performance Dashboard.pbix` open, the file saves as `Sales Performance Dashboard_ModelExport.json`.

---

## What Gets Exported

| Section | Contents |
|---------|----------|
| **Model Metadata** | Compatibility level, culture, default mode (Import/DirectQuery), object counts |
| **Tables** | Name, description, visibility, auto-generated flag, resolved source folder path, data category, table type (Regular/CalculatedTable), partition source types |
| **Columns** | Name, data type, column type (Data/Calculated/CalculatedTableColumn), key status, format string, display folder, data category, summarize-by, sort-by-column |
| **Measures** | Name, full DAX expression, description, data type, format string, display folder, visibility, top-level KPI flag, direct measure dependencies, full recursive dependency chain |
| **Partitions** | Name, source type (M/Calculated/Entity), full M query or DAX expression, storage mode |
| **Hierarchies** | Name, levels with ordinal positions and source columns |
| **Relationships** | From/to table and column, cardinality, active/inactive, cross-filter direction, security filtering, fact/dimension role hints |
| **Roles (RLS)** | Role name, description, permission level, DAX filter expressions per table |
| **Data Sources** | Name, description, type |
| **Summary** | User-facing vs auto-generated table split, top-level KPI list, measures grouped by display folder, relationship map, column inventory per table, measure counts per table |
| **Data Head** | First N rows sampled from each table's source file: column names and raw cell values |

---

## Data Head

The `dataHead` section reads source files directly from disk: no ADOMD connection, no ACE OLEDB driver, no Office installation required.

**Supported formats:**

| Format | Method |
|--------|--------|
| `.csv` | Native delimiter split |
| `.tsv` | Native tab split |
| `.txt` | Native delimiter split |
| `.xlsx` | Open XML ZIP parsing via `ZipArchive` + `XmlDocument` |

**OneDrive path resolution:** source paths are stored in M expressions with the original author's username and OneDrive tenant name baked in. The script resolves them dynamically on whoever's machine is running it, using a three-strategy fallback:

1. Exact path match (same machine, same user)
2. Rebuild path using `OneDriveCommercial` / `OneDrive` / `OneDriveConsumer` environment variables, which handles username and tenant name differences
3. Folder name search under OneDrive roots and common profile paths, as a last resort if the directory structure has changed

If the source folder can't be resolved, the `dataHead` entry returns an `error` key with a descriptive message rather than crashing the export.

**Data head output example:**

```json
"dataHead": {
  "Sales": {
    "sourceFile": "Sales_FY2025.xlsx",
    "columns": ["Region", "Salesperson", "Product", "Quarter", "Revenue", "Units", "Cost", "Margin"],
    "rows": [
      ["Northeast", "Sarah Kim", "Enterprise License", "Q1", "142500.00", "3", "87000.00", "0.389"],
      ["Southwest", "Marcus Rivera", "Professional Tier", "Q1", "48750.00", "15", "29250.00", "0.400"]
    ]
  }
}
```

> **Note on numeric precision:** XLSX stores floating point values at full IEEE 754 precision. Decimal values may appear as scientific notation strings (e.g. `3.9E-1`). Parse as `double` and round downstream as needed.

---

## Output Format

```json
{
  "exportDate": "2026-03-15 09:22:41",
  "dashboardName": "Sales Performance Dashboard",
  "modelName": "a3f92c10-7d44-4e81-b312-9f0c8e45aa12",
  "modelMetadata": {
    "compatibilityLevel": 1600,
    "culture": "en-US",
    "defaultMode": "Import",
    "tableCount": 4,
    "relationshipCount": 3,
    "measureCount": 31,
    "roleCount": 1
  },
  "exportConfiguration": {
    "includeHiddenObjects": true,
    "includePartitionSources": true,
    "includeRoles": true,
    "headRowCount": 50
  },
  "tables": [ ... ],
  "relationships": [ ... ],
  "roles": [ ... ],
  "dataSources": [ ... ],
  "summary": {
    "userFacingTables": ["Sales", "Products", "Regions", "Targets"],
    "autoGeneratedTables": [],
    "topLevelKPIs": ["Revenue vs Target", "YTD Revenue", "Margin %", "Win Rate"],
    "measuresByFolder": {
      "00 - KPIs": ["Total Revenue", "Total Units", "Active Accounts"],
      "01 - Targets": ["Revenue vs Target", "Attainment %"],
      "02 - Trend": ["YTD Revenue", "3yr Avg Revenue", "Revenue Growth"]
    },
    "relationshipMap": [
      "Sales.ProductID --> Products.ProductID (Many:One)",
      "Sales.RegionID --> Regions.RegionID (Many:One)"
    ],
    "columnInventory": {
      "Sales": ["OrderID (Int64)", "Revenue (Double)", "Units (Int64)", "Quarter (String)", "RegionID (Int64)"],
      "Products": ["ProductID (Int64)", "ProductName (String)", "Category (String)", "ListPrice (Double)"]
    },
    "measuresPerTable": {
      "Sales": 31
    }
  },
  "dataHead": {
    "Sales": {
      "sourceFile": "Sales_FY2025.xlsx",
      "columns": [ ... ],
      "rows": [ ... ]
    }
  }
}
```

---

## Integration Examples

### Feed to an AI Assistant

Upload the JSON file directly to Claude, ChatGPT, or any LLM and ask questions like:

- "Review my DAX measures for performance issues"
- "What does the actual data look like, and what are the distinct values in Region?"
- "What happens if I rename the ProductID column?"
- "Suggest measures I'm missing for a sales performance dashboard"
- "Document this model for my team"
- "Which top-level KPIs depend on the Total Revenue base measure?"

### Python Analysis

```python
import json

with open("Sales_Performance_Dashboard_ModelExport.json", "r", encoding="utf-8") as f:
    model = json.load(f)

print(f"Dashboard: {model['dashboardName']}")
print(f"Tables: {model['modelMetadata']['tableCount']}")
print(f"Measures: {model['modelMetadata']['measureCount']}")

# User-facing tables only
print("\nUser-facing tables:")
for t in model["summary"]["userFacingTables"]:
    print(f"  {t}")

# Top-level KPIs
print("\nTop-level KPIs:")
for kpi in model["summary"]["topLevelKPIs"]:
    print(f"  {kpi}")

# Data head: print first row of each table
print("\nData head sample:")
for table_name, head in model["dataHead"].items():
    if "rows" in head and head["rows"]:
        cols = head["columns"]
        row  = head["rows"][0]
        print(f"\n  {table_name}")
        for col, val in zip(cols, row):
            print(f"    {col}: {val}")

# Measures with deep dependency chains
print("\nComplex measures:")
for table in model["tables"]:
    for m in table["measures"]:
        chain = m["fullDependencyChain"]
        if len(chain) >= 3:
            print(f"  {m['name']} -> {len(chain)} upstream measures")

# Fact vs dimension tables from relationships
print("\nRelationship roles:")
for r in model["relationships"]:
    print(f"  Fact: {r['factTable']} | Dimension: {r['dimensionTable']}")
```

### Power Query Import

```powerquery
let
    Source = Json.Document(File.Contents("Sales_Performance_Dashboard_ModelExport.json")),
    Tables = Source[tables],
    TableList = Table.FromList(Tables, Splitter.SplitByNothing()),
    Expanded = Table.ExpandRecordColumn(TableList, "Column1",
        {"name", "tableType", "isHidden", "isAutoGenerated", "sourceFolder", "columns", "measures"})
in
    Expanded
```

---

## File Locations

The script automatically saves to your Downloads folder, named after the open report:

| OS | Path |
|----|------|
| Windows | `C:\Users\{username}\Downloads\{ReportName}_ModelExport.json` |
| Mac | `/Users/{username}/Downloads/{ReportName}_ModelExport.json` |
| Linux | `/home/{username}/Downloads/{ReportName}_ModelExport.json` |

The output folder is created automatically if it doesn't exist.

---

## Troubleshooting

**Script compiles but output is empty:**
Check that your model has tables. Open the Tables pane in Tabular Editor to verify the model loaded.

**Dashboard name shows as "UnknownReport":**
The script reads the Power BI Desktop window title. Make sure the report is open and fully loaded in Power BI Desktop before running the script in Tabular Editor.

**`dataHead` shows `"error": "Folder not found"`:**
The source folder path couldn't be resolved on the current machine. Make sure OneDrive is synced and the source data folder is available locally (right-click → "Always keep on this device"). The script will retry automatically using OneDrive environment variables and folder name search before surfacing this error.

**`dataHead` shows `"note": "Unsupported format"`:**
The source file is not CSV, TSV, TXT, or XLSX. The script returns a file list instead of row data for unsupported binary formats.

**XLSX numeric values in scientific notation:**
This is expected. XLSX stores full IEEE 754 precision in the XML. Parse the string as `double` and apply rounding downstream.

**"Expression" is blank on partitions:**
Some partition types (e.g. `Entity` in DirectQuery) don't expose source expressions. The script catches this cleanly and the field will be an empty string.

**`sourceFolder` is empty:**
Only tables loaded via `Folder.Files()` or `File.Contents()` in their M expression will have this populated. SQL, SharePoint, and other source types won't produce a folder path.

**Hidden tables/columns missing:**
Set `includeHiddenObjects = true` in the configuration section.

**File not appearing in Downloads:**
Check the Tabular Editor output pane for the full path. The script prints the output location on success.

---

## Technical Details

### Data Head: XLSX Parsing

XLSX files are ZIP archives containing XML. The script reads them directly using `ZipArchive` (part of `System.IO.Compression`) and `XmlDocument` (part of `System.Xml`), both available natively in TE2's .NET runtime with no external references.

Two internal files are read:

- `xl/sharedStrings.xml`: Excel de-duplicates all string values into a lookup table; cell values with `type="s"` are resolved by index against this table
- `xl/worksheets/sheet1.xml`: cell data for the first worksheet; row 0 is treated as the header row

### OneDrive Path Resolution

M expressions store the absolute path of the source folder as it existed on the original author's machine. The resolver uses three strategies in order:

1. **Exact match:** try the path verbatim
2. **Environment variable rebuild:** strip the stored username and OneDrive tenant segment, then reattach the real local OneDrive root from `OneDriveCommercial`, `OneDrive`, or `OneDriveConsumer` env vars
3. **Folder name search:** recursively search for the target folder name under all OneDrive roots and common profile paths

### Measure Dependency Detection

Direct dependencies are extracted using regex bracket-token matching (`\[([^\]]+)\]`) against a pre-built `HashSet` of all measure names. Full recursive dependency chains are resolved by walking the dependency graph with circular reference protection.

### Top-Level KPI Detection

A reverse lookup is built across all measure expressions before export. Any measure whose name never appears as a dependency in another measure's expression is flagged `isTopLevelKPI: true`. These are your model's user-facing entry points.

### Auto-Generated Table Detection

Tables whose names contain a GUID pattern are flagged `isAutoGenerated: true` and surfaced separately in the summary so AI can deprioritize them.

### Relationship Role Hints

Each relationship includes `factTable` and `dimensionTable` fields derived from cardinality: the `Many` side is the fact table, the `One` side is the dimension table.

### Output Encoding

UTF-8 without BOM (`new UTF8Encoding(false)`) for maximum compatibility with JSON parsers, Python, and web tools.

---

## Changelog

### Current

- **Data head:** first N rows sampled directly from source files, no ADOMD or ACE OLEDB required
- **XLSX support:** Open XML parsed via `ZipArchive` + `XmlDocument`, works without Office installed
- **Dynamic OneDrive path resolution:** three-strategy resolver handles username, tenant name, and directory structure differences across machines
- `sourceFolder` field on each table (replaces `sourceFilePath`, now resolves to the folder, not the individual file)
- `headRowCount` added to `exportConfiguration` section
- Assembly reference `#r "System.IO.Compression.dll"` for TE2 compatibility
- Removed version numbering from script output

### v3.0

- Auto-detects report name from Power BI Desktop window title
- `isAutoGenerated` flag on tables containing GUIDs
- `sourceFilePath` field extracted from M partition expressions
- `isTopLevelKPI` flag per measure
- `fullDependencyChain` per measure with circular reference protection
- `factTable` / `dimensionTable` role hints on relationships
- Summary expanded with `userFacingTables`, `autoGeneratedTables`, `topLevelKPIs`, `measuresByFolder`

### v2.0

- Full model export: tables, columns, relationships, partitions, hierarchies, roles, data sources
- Proper JSON escaping for all control characters
- Regex-based measure dependency detection
- Comma-safe output using list-join pattern
- UTF-8 without BOM

### v1.0

- Measures and calculated columns only
- Basic string-replace JSON escaping
- Manual comma tracking

---

## License

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

You are free to use, share, and adapt this work, including at your job, under these terms:

- **Attribution:** Credit the original author
- **NonCommercial:** No selling or commercial products
- **ShareAlike:** Derivatives must use the same license
