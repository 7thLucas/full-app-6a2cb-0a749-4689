# BLACKTOC — Design System

## Color Palette
- **Primary Background**: `#000000` (pure black)
- **Secondary Background**: `#111111`, `#1a1a1a`, `#1f1f1f`
- **Card/Surface**: `#18181b` (gray-900), `#27272a` (gray-800)
- **Gold Accent (Primary CTA)**: `#F59E0B` (amber-500)
- **Gold Accent (Hover/Deep)**: `#D97706` (amber-600)
- **Gold Accent (Light)**: `#FCD34D` (amber-300) for subtle highlights
- **Text Primary**: `#FFFFFF`
- **Text Secondary**: `#A1A1AA` (zinc-400)
- **Text Muted**: `#52525B` (zinc-600)
- **Success**: `#22C55E` (green-500)
- **Error**: `#EF4444` (red-500)
- **Warning**: `#F59E0B` (amber-500)
- **Live Badge**: `#EF4444` pulsing red
- **Border**: `#3F3F46` (zinc-700)

## Typography
- **Font Family**: Inter (Google Fonts) — clean, modern, readable
- **Display/Hero**: 800 weight, tight tracking
- **Headings**: 700 weight
- **Body**: 400 weight, relaxed line-height
- **Captions/Labels**: 500 weight, uppercase tracking for labels

## Elevation / Depth
- Cards use subtle gold border on hover (`border-amber-500/30`)
- Glass morphism on overlays: `backdrop-blur-sm bg-black/60`
- Modals: `bg-gray-900 border border-gray-800 rounded-2xl`
- Toasts: slide in from top-right, dark with gold left-border accent

## Component Patterns
- **Buttons (Primary)**: `bg-amber-500 hover:bg-amber-600 text-black font-bold rounded-full px-6 py-3`
- **Buttons (Secondary)**: `bg-gray-800 hover:bg-gray-700 text-white border border-gray-700 rounded-full`
- **Buttons (Ghost)**: `text-amber-500 hover:text-amber-400 underline-offset-4`
- **Input Fields**: `bg-gray-900 border border-gray-700 focus:border-amber-500 rounded-xl text-white`
- **Video Cards**: Vertical aspect ratio (9:16 thumbnail), dark overlay gradient, creator info at bottom
- **Stat Cards**: Dark surface, gold number, gray label, subtle glow on hover
- **Badge/Tag**: `bg-amber-500/20 text-amber-400 rounded-full text-xs px-2 py-0.5`
- **Avatar**: Circular, gold ring on verified creators (`ring-2 ring-amber-500`)

## Layout
- **Mobile**: Full-screen video swipe (TikTok-style), bottom nav bar (5 items)
- **Desktop**: Left sidebar nav (240px), main content area, optional right rail
- **Bottom Nav (Mobile)**: Home, Explore, Upload (+), Notifications, Profile — icons + labels
- **Sidebar (Desktop)**: BLACKTOC logo + gold wordmark, nav items with icons, earnings widget at bottom

## Motion / Animation (Framer Motion)
- Feed scroll: smooth spring transition between video cards
- Page transitions: fade + slide up (0.3s ease-out)
- Like button: heart burst animation (scale + color flash)
- Earnings counter: animated number roll-up
- Toast notifications: slide in from right, auto-dismiss after 4s
- Live badge: pulsing red dot animation
- Coin/gift animations: particle burst effect

## Mobile-First Responsive
- Base styles target 375px (iPhone SE)
- `md:` breakpoint for tablet (768px)
- `lg:` breakpoint for desktop (1024px)
- Video feed: full viewport height on mobile (`h-[100dvh]`)
- Bottom nav hidden on desktop; sidebar hidden on mobile

## Iconography
- Use `lucide-react` for all icons (consistent, clean)
- Gold accent on active nav items
- Filled variants for active state, outline for inactive

## Special UI Elements
- **Creator Health Score**: Circular progress ring in gold
- **Earnings Ticker**: Animated counter with gold text
- **Viral Alert Toast**: Gold border, fire emoji, milestone text
- **Live Stream**: Full-screen dark layout with chat overlay on right
- **Coin Display**: Gold coin icon + formatted number
- **Verification Badge**: Gold checkmark (verified creators)
- **League Badge**: Tiered color (Bronze/Silver/Gold/Platinum/Diamond)
