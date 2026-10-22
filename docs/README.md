# Merge conflict evidence

Screenshots captured while attempting to merge `feature-green-button` into `main`
after `feature-red-button` had already been merged (Practical 4, Part 7).

| File | Content |
| --- | --- |
| `conflict-evidence-pr2-page.png` | Pull Request #2 page showing *"This branch has conflicts that must be resolved"* |
| `conflict-evidence-compare-banner.png` | Compare view showing *"Can't automatically merge"* |

The conflict occurred because both branches changed the same attribute
(`android:backgroundTint`) on the same lines of
`app/src/main/res/layout/activity_main.xml`:

- `feature-red-button`: `#F44336` (red)
- `feature-green-button`: `#4CAF50` (green)

The conflict was resolved with Option C — the group agreed to keep both colours:

- `firstButton`: `#F44336` (red)
- `secondButton`: `#4CAF50` (green)

Resolution commit: `Resolve button color merge conflict`.
