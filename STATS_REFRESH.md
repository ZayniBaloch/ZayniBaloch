# GitHub Stats Cache Refresh
# This file helps refresh GitHub stats by triggering a rebuild

## How to Force Refresh GitHub Stats:

### Method 1: Manual Cache Bust
Add `?cache_seconds=1800` to force refresh every 30 minutes.

### Method 2: Force Refresh URLs
For immediate refresh, append `&v=` + current timestamp to stats URLs.

### Method 3: GitHub Actions Auto-refresh
The snake animation workflow runs every 12 hours and updates stats.

## Current Stats Configuration:
- **Cache Duration**: 30 minutes (1800 seconds)
- **Include Private Repos**: ✅ Yes
- **Include All Commits**: ✅ Yes
- **Theme**: Tokyo Night
- **Real-time Updates**: ✅ Enabled

## Refresh Commands:
```bash
# Force refresh by creating empty commit
git commit --allow-empty -m "🔄 Force refresh stats" && git push

# Manual trigger snake workflow
gh workflow run snake.yml
```

## Stats Services Used:
1. **GitHub Readme Stats** - Main stats cards
2. **GitHub Streak Stats** - Contribution streaks  
3. **GitHub Profile Summary Cards** - Detailed breakdowns
4. **GitHub Activity Graph** - Contribution heatmap
5. **GitHub Profile Trophy** - Achievement trophies

---
*Last Updated: August 18, 2025*
