# Transform Map Configuration

## Source
Import Set Table created from the spreadsheet.

## Target
Incident table (`incident`) or the target table specified by the project.

## Suggested Transform Map
**Name:** Import Incident Data from Spreadsheet

### Field Maps

| Source | Target |
|---|---|
| Number | Number |
| Short description | Short description |
| Description | Description |
| Caller | Caller |
| Priority | Priority |
| State | State |

## Coalesce
If the project requires updating an existing record instead of creating a duplicate, configure a suitable unique source field as **Coalesce**.

Example:
- Source field: `Number`
- Coalesce: `true`

Only use Coalesce when the source value corresponds to a unique target value in the instance.

## Transform
1. Open the created Transform Map.
2. Verify all field maps.
3. Click **Transform**.
4. Review the transform result.
5. Check **Transform History** for errors or ignored rows.

## Validation
Confirm:
- Records were created/updated.
- Required fields contain valid values.
- Reference fields resolve correctly.
- Choice fields contain accepted values.
- No unexpected duplicate records were created.
