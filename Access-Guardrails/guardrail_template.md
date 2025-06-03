# Access Guardrail Policy Template

## Fields
- **Data Table**: Name of the dataset or table (e.g., sipp_user_data)
- **Allowed Columns**: List of approved fields (e.g., email, region)
- **Requester Role**: e.g., Security Engineer, Data Analyst
- **Max Duration**: e.g., 30 days, 1 year
- **Approval Needed From**: L10 leader, Security Owner, etc.

## Sample Policy (JSON)
```json
{
  "table": "sipp_user_data",
  "allowed_columns": ["user_id", "region", "account_status"],
  "requester_role": "SecurityEngineer",
  "max_duration_days": 365,
  "approval_required": ["L10Leader", "SecurityProductOwner"]
}
