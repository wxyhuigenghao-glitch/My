# Charging revision visual QA

final result: passed

Source visual truth: /var/folders/9j/krjfmr1s2xjbg523z9bbx83r0000gn/T/codex-clipboard-a825630d-20b1-451d-ae0b-4dca50c6c21c.png (2082 × 1120), with the user's annotated screenshot and explicit supercar request.
Implementation screenshots: /Users/wengxinyu/Documents/AIdocs/personal-site/.preview/charging-desktop.png, charging-results.png, charging-rotated.png, charging-mobile.png.
Viewport: 1512 × 982 desktop; 390 × 844 mobile, full-page capture. DPR 1. Wireframe depicts a portrait control surface, adapted inside the existing landscape composition; not a pixel-exact whole-page comparison.

Full-view comparison: reference wireframe and desktop/mobile renders opened together. Control-region text remains readable at supplied resolution, so separate detail crops were unnecessary.

Structure verified: charge/discharge/settings tabs; service tag; combined status and percentage band; remaining time and power; stop button; central vehicle; Bluetooth status; single-line total/electric/fuel mileage; four controls; three reservation cards. Removed orbit/reset/fullscreen controls, drag instruction, and decorative scene title. Continuous dark background retained.

Required fidelity surfaces:
- Typography: existing site fonts preserved; lower mileage values now inline with labels rather than large stacked metrics.
- Spacing/layout: cards below four controls; no dividing border in the mileage/control area; no collisions in final desktop capture.
- Colors: original immersive dark green and green pulse preserved, translucent status band follows wireframe.
- Asset: SUV replaced with a procedural, low-slung supercar including curved body, canopy, wide wheels, narrow lights and rear wing. It is an original concept, not an exact branded model.
- Content: research/results unchanged; scene text limited to prototype functions and reservation state.

Iteration history:
1. P2: first supercar render overlapped mileage; corrected camera framing and enlarged model while moving it up.
2. P2: body surface winding inverted; corrected mesh triangle order and checked final screenshot.
3. Final recapture showed no remaining P0/P1/P2 layout or functional issue.

Verification: no JavaScript page errors; WebGL canvas rendered; research/results, charge stop/start, discharge, charge reservation, use-car reservation, drag rotation, removed-control absence, and mobile horizontal overflow checks passed. Chrome fallback used because in-app automation previously failed during runtime startup.

Remaining P3: production CAD could provide more realistic vehicle body surfacing. No external model is required for the standalone HTML.

## Revision: collapsible narrative and source slides

final result: passed

New source: user references codex-clipboard-4f564862-dca6-4784-9007-e3e57c45f06a.png (black backlit vehicle and side/angled states), codex-clipboard-18f4156d-3e0c-40f8-af70-ed442a760aa5.png (research data); original research/results slide images embedded unchanged as data URLs.
Evidence: .preview/charging-collapsed.png and charging-desktop.png viewed together at 1512×982, DPR 1; charging-slide.png inspected for full original-image readability; charging-mobile.png inspected at 390px width.
Typography/layout: role sentence below slogan; tab-specific original-slide action at bottom left; chart labels readable; folded panel inert and unavailable to keyboard; panel opens horizontally on landscape screens and stacks on mobile.
Colors/assets: neutral black body, white rear rim lights, green energy environment retained. Side angle starts at 0 and eases to -π/4 only with narrative expansion. All pointer-controlled model rotation removed. Vehicle remains a procedural concept model.
Data: pie uses the source's explicit 30% private ownership, with its 70% complement; avoids repeating inconsistent duplicated 30% source labels. Bars show supported 60% daily-twice and >50% in-car figures; second bar explicitly labeled as a 50% lower-bound illustration. They are independent measures, not a shared population breakdown.
Interactions tested: starts collapsed, expand, collapse, reopen; both tab-specific original images load/decode, correct titles, Escape and close button; energy controls and reservation regression; mobile overflow. No JS errors. Reduced-motion users get immediate vehicle angle changes and CSS animation suppression.
No remaining P0/P1/P2 findings for this revision. Existing P3 vehicle-surface fidelity limitation remains.

## Revision: U8-style vehicle and indoor parking

final result: passed

Source: latest supplied cable detail (ade3db49), U8 photo (d67900fc), and indoor charging scene (35b1ab23). Final desktop screenshot and indoor reference inspected together. Desktop 1512×982 DPR1; collapsed and expanded states captured, mobile overflow tested.
Changes: exact requested slogan replaces old slogan and paragraph; top-right microcopy removed. Collapsed column width is zero, and toggle floats at 50vh with no rail. Rebuilt car with reference-led U8 proportions, rear spare, patterned grille, split lights, squared fenders; retains black backlit finish. This is an approximate procedural reconstruction rather than an OEM CAD asset. Replaced exterior grid with concrete wall panels, columns, ceiling geometry and parking lines. Charging cable now has continuous subdued green emissive shading, diffuse surrounding glow and floor light; no separate pulse beads or white rings.
QA iteration: initial cable glow layers were too conspicuous; reduced halo opacity from .07 to .018 and emission from .5 to .24. Added top scene fade to remove a hard header edge. Raised neutral key light slightly to reveal black body contours. Recaptured final view and checked content, type, spacing, background continuity and lighting.
Regression: collapsed startup, expand/collapse, both original PPT dialogs, original image decode, research/results tabs, charging/discharging, both reservation controls, mobile overflow; no JavaScript page errors. Existing limitation: vehicle surface detail is stylized, not photorealistic.

## Revision: charging pedestal and energy pulses

final result: passed

Reference: latest charging pedestal images (4161bc31 and 1a60471c) and concentric floor pulse image (13b3d9c4). Reference pulse image and collapsed screenshot opened together; expanded screenshot also inspected at 1512×982 DPR1.
Added fixed pedestal, inset battery/status screen, illuminated trim and socket; cable curves are recalculated as the car turns so both endpoints remain connected. Green pulses travel along the cable surface via shader; three expanding green rings and broad soft light spread across the floor. All energy shaders and floor point light are disabled on pause and when discharging.
Vehicle polish: rounded box geometry for larger components, finer profile bevels, studio environment reflection, reduced windshield reflection intensity, adjusted black paint roughness and metalness. No change of vehicle identity: reference-led U8-style reconstruction remains approximate.
QA: no overlaps of primary UI in collapsed/expanded renders. Preserved narrative, charts, original slide viewers and indoor background. Full interaction regression passed with zero page errors. Separate screenshot-region comparison confirmed active pulse frames differ, paused frames remain identical, and resumed frame changes again. Evidence: charging-collapsed.png, charging-desktop.png, charging-paused.png.
Remaining P3: OEM-grade body surfacing would require a detailed original model; current geometry is a stylized interactive reconstruction.

## Revision: concise English overview and tighter controls

final result: passed

Four vehicle controls now occupy a centered 480px maximum-width group with 8px grid gaps, retaining mobile fit. Project overview copy, tabs, charts, slide controls and accessible labels translated into concise English; original source images retained. Added requested top-right text: “Not the company’s original design. Adapted to remove confidential information.”
Verified desktop 1512×982 screenshot and mobile 390px layout. English overview checked for untranslated Chinese text; disclosure visibility and page width passed. Existing interaction regression passed with zero page errors. Latest screenshot: .preview/charging-desktop.png; mobile: .preview/charging-english-mobile.png.

## Revision: single-line heading and reservation popover

final result: passed

Title now stays on one line at responsive sizes. Role starts with “My role:”; “CASE STUDY” removed. Reservation cards are hidden on initial load and opened through the centered 设置预约 button; Escape, outside clicks and toggle close them. Saved reservation values survive closing/reopening during the session. No fabricated pre-existing bookings introduced.
Desktop default and expanded reservation screenshots inspected at 1512×982; single-line title, compact controls, and floating reservation cards fit. Mobile overflow check and existing charge/time/trip/PPT regressions passed; zero page errors. Evidence: .preview/charging-desktop.png, charging-results.png, charging-mobile.png.

## Revision: in-flow reservation expansion

final result: passed

Reservations now occupy space in the bottom flex stack (mileage → controls → cards → toggle) rather than overlaying controls. The expanding max-height smoothly raises mileage and controls; collapse restores their positions. Hidden cards are inert. Bluetooth authentication label removed as requested.
Verification: .preview/charging-reservations-expanded.png visually inspected at 1512×982. Bounding-box checks confirm mileage moves upward, card top stays below control bottom, saving works and collapse restores original position. Mobile width check passed. The first timing-sensitive assertion sampled an unfinished animation; a second capture and geometry check confirmed the intended movement and no overlap.
