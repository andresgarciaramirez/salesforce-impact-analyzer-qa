# Changelog

## 0.1.0 — first public version

- Impact ("where used") of a field or a whole object in an org authenticated in the Salesforce CLI.
  No credentials are requested or stored.
- Two sources, each finding labelled with its source and type:
  - Dependency API (Tooling `MetadataComponentDependency`), queried through both the Tooling query
    and Bulk API 2.0 (each route misses things the other returns);
  - source scan: selective Metadata API retrieve, unzipped and scanned in memory.
- Covers fields (formulas, roll-ups, lookups, dependencies), validation rules, flows and Process
  Builder, workflow rules/field updates/alerts, Apex classes/triggers, Visualforce, LWC/Aura, page
  and compact layouts, record types, list views, field sets, reports, report types, email
  templates, Lightning pages, quick actions, buttons/links, approval processes, sharing and
  assignment rules, duplicate rules and paths.
- Honest coverage section in every report (status of each source, reliability per type, what
  neither source can see). "No references" is never presented as "safe".
- Report view, sidebar summary, Markdown/HTML/CSV export. English and Spanish.
- Read-only, 100% local: no backend, no telemetry; credentials and metadata are never logged or
  persisted.
