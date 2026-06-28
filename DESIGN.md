# Kerwin Profile Design System

## 1. Atmosphere & Identity

An executive AI product flight deck: calm, precise, evidence-led, and international. The signature is the Evidence Flight Deck, a dark technical panel that frames Kerwin's work as a loop from data quality to evaluation to cloud-native delivery.

## 2. Color

### Palette

| Role | Token | Light | Dark | Usage |
|------|-------|-------|------|-------|
| Surface/primary | `ink-950` | `#F8FAFC` | `#08111F` | README hero and dark panels |
| Surface/secondary | `slate-900` | `#E6EEF7` | `#102033` | Secondary SVG panels |
| Surface/elevated | `mist-100` | `#F3F8FB` | `#D9E8EF` | Light stats surfaces |
| Text/primary | `ice-50` | `#FFFFFF` | `#FFFFFF` | Hero headings |
| Text/secondary | `fog-300` | `#A9BBC8` | `#A9BBC8` | Captions and metadata |
| Accent/primary | `cloud-400` | `#55C7F3` | `#55C7F3` | AI/product signal |
| Accent/quality | `jade-400` | `#39D98A` | `#39D98A` | Data quality and validation |
| Accent/research | `violet-400` | `#A78BFA` | `#A78BFA` | Research and benchmark signal |
| Line/subtle | `line-500` | `#28445C` | `#28445C` | SVG circuit lines |

### Rules

- Dark surfaces are used only for the signature hero asset.
- Accent colors encode the user's real work: cloud, data quality, and research.
- Avoid generic purple-blue gradient backgrounds; gradients must look like instruments, not marketing haze.

## 3. Typography

### Scale

| Level | Size | Weight | Line Height | Tracking | Usage |
|-------|------|--------|-------------|----------|-------|
| Display | 72px | 780 | 1.0 | 0 | SVG nameplate |
| H1 | GitHub default | 700 | GitHub default | 0 | README title fallback |
| H2 | GitHub default | 600 | GitHub default | 0 | Section headings |
| Body | GitHub default | 400 | GitHub default | 0 | README body |
| Caption | 11px | 600 | 1.4 | 0.08em | SVG labels |
| Utility | 13px | 500 | 1.4 | 0.04em | SVG metrics and chips |

### Font Stack

- Primary: GitHub system sans in README rendering.
- SVG display: `ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif`.
- SVG utility: `ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace`.

### Rules

- The SVG carries the custom typography; README body stays GitHub-native for reliability.
- No emoji icons. Labels and linework carry the visual system.

## 4. Spacing & Layout

### Base Unit

All spacing derives from 4px.

| Token | Value | Usage |
|-------|-------|-------|
| `space-2` | 8px | Tight labels |
| `space-3` | 12px | SVG chip padding |
| `space-4` | 16px | Compact panel padding |
| `space-6` | 24px | Default panel padding |
| `space-8` | 32px | Hero internal rhythm |
| `space-12` | 48px | Section breaks |

### Grid

- README layout: single-column GitHub Markdown, with evidence lists for mobile readability.
- SVG layout: left nameplate, right three-node loop, bottom proof rail.

### Rules

- Avoid Markdown tables for core profile content because they degrade on mobile GitHub views.
- Avoid nested card grids in README; the signature asset is the only dense visual object.

## 5. Components

### Evidence Flight Deck

- **Structure**: local SVG image referenced from README.
- **Variants**: one hero variant only.
- **Spacing**: `space-4`, `space-6`, `space-8`.
- **States**: static, because GitHub README strips interactive script.
- **Accessibility**: README supplies alt text; SVG includes title and desc.
- **Motion**: none in GitHub profile context.

### Signal Brief

- **Structure**: Markdown bullet list with a bold signal, one product sentence, and one proof sentence.
- **Variants**: research, infra, cloud, documentation.
- **Spacing**: GitHub list default.
- **Accessibility**: text-first, no image-only claims.
- **Motion**: none.

## 6. Motion & Interaction

GitHub README is static. The high-end feel comes from composition, precision, and restrained visual density rather than animation.

## 7. Depth & Surface

### Strategy

Mixed inside the SVG only: dark tonal shifts, subtle strokes, and low-opacity accent glows. README body uses GitHub native surfaces.
