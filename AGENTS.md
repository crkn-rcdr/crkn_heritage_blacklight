# Heritage Blacklight Guidelines

1. **Selective Cherry-Pick Only**:
   - Never perform blind `git merge upstream/master` or `git merge upstream/main`.
   - Never click GitHub's web "Sync fork" button.
   - Only selectively cherry-pick specific commit SHAs from `crkn_base_blacklight`.

2. **Safeguard Themes & Labels**:
   - Never allow upstream base to overwrite `config/locales/` (preserve "reels" vs "issues" labeling and archival terms).
   - Never allow upstream base to overwrite `app/assets/stylesheets/base/canadiana.scss` (preserve Heritage Forest Green `#338500` theme and layouts).
   - Never overwrite Solr external float filter `{!frange l=1}has_full_text_eff` in `app/controllers/catalog_controller.rb`.

3. **Mandatory Inventory Update**:
   - Whenever any Heritage-specific customization is created, modified, or removed, **always update** the inventory checklist located at:
     `/home/brittny/github/platform2-local/.agents/skills/crkn-blacklight/references/heritage-customizations-inventory.md`
   - Document any new locale keys, CSS variables, queries, or template adjustments so future upstream syncs never overwrite them.

