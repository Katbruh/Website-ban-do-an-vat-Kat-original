# Decisions

Append-only, ADR-style (spec 7.9): one entry per decision, newest last. A later entry for the same path supersedes an earlier one; nothing is edited or deleted. set_by is chosen, confirmed_default, auto_default, assumed, delegated, reference, asset or standard.

## D-0001 · init with defaults
- set_by: auto_default · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: Start of the design system; every default traces to references/levers.json.

## D-0002 · House standards v3: 455 applied
- set_by: standard · locked: yes · date: 2026-11-04 · supersedes: none · source_ref: standards.json v3
- reason: OpenDesigner's house standards (sources marked non-negotiable) are applied without asking and locked. Change one only when the person asks: engine.py standard override <id> --why "<their words>".
- <details><summary>455 standards</summary> STD-when-to-animate-01, STD-when-to-animate-03, STD-when-to-animate-04, STD-when-to-animate-05, STD-when-to-animate-06, STD-when-to-animate-07, STD-when-to-animate-08, STD-when-to-animate-09, STD-when-to-animate-10, STD-when-to-animate-11, STD-when-to-animate-13, STD-when-to-animate-14, STD-when-to-animate-15, STD-when-to-animate-16, STD-when-to-animate-17, STD-when-to-animate-20, STD-when-to-animate-22, STD-easing-duration-01, STD-easing-duration-02, STD-easing-duration-03, STD-easing-duration-06, STD-easing-duration-07, STD-easing-duration-09, STD-easing-duration-10, STD-easing-duration-11, STD-easing-duration-12, STD-easing-duration-13, STD-easing-duration-15, STD-easing-duration-17, STD-easing-duration-19, STD-enter-exit-origin-01, STD-enter-exit-origin-02, STD-enter-exit-origin-03, STD-enter-exit-origin-04, STD-enter-exit-origin-06, STD-enter-exit-origin-08, STD-enter-exit-origin-09, STD-enter-exit-origin-10, STD-enter-exit-origin-11, STD-enter-exit-origin-12, STD-enter-exit-origin-13, STD-enter-exit-origin-16, STD-enter-exit-origin-17, STD-enter-exit-origin-21, STD-enter-exit-origin-23, STD-enter-exit-origin-24, STD-enter-exit-origin-25, STD-enter-exit-origin-26, STD-enter-exit-origin-27, STD-enter-exit-origin-28, STD-enter-exit-origin-29, STD-enter-exit-origin-30, STD-enter-exit-origin-31, STD-enter-exit-origin-33, STD-enter-exit-origin-34, STD-enter-exit-origin-35, STD-enter-exit-origin-37, STD-enter-exit-origin-38, STD-enter-exit-origin-39, STD-enter-exit-origin-40, STD-enter-exit-origin-41, STD-enter-exit-origin-42, STD-enter-exit-origin-43, STD-enter-exit-origin-44, STD-springs-gestures-01, STD-springs-gestures-02, STD-springs-gestures-04, STD-springs-gestures-05, STD-springs-gestures-06, STD-springs-gestures-07, STD-springs-gestures-08, STD-springs-gestures-09, STD-springs-gestures-10, STD-springs-gestures-11, STD-springs-gestures-12, STD-springs-gestures-13, STD-springs-gestures-14, STD-springs-gestures-15, STD-springs-gestures-16, STD-springs-gestures-17, STD-springs-gestures-18, STD-springs-gestures-19, STD-springs-gestures-20, STD-springs-gestures-21, STD-springs-gestures-22, STD-springs-gestures-23, STD-springs-gestures-24, STD-springs-gestures-25, STD-springs-gestures-26, STD-springs-gestures-28, STD-springs-gestures-30, STD-springs-gestures-34, STD-springs-gestures-39, STD-springs-gestures-41, STD-springs-gestures-42, STD-springs-gestures-45, STD-springs-gestures-59, STD-springs-gestures-60, STD-springs-gestures-61, STD-springs-gestures-63, STD-performance-properties-01, STD-performance-properties-02, STD-performance-properties-06, STD-performance-properties-09, STD-performance-properties-10, STD-performance-properties-11, STD-performance-properties-12, STD-performance-properties-13, STD-performance-properties-14, STD-performance-properties-15, STD-performance-properties-16, STD-performance-properties-17, STD-performance-properties-18, STD-performance-properties-19, STD-performance-properties-20, STD-performance-properties-24, STD-performance-properties-25, STD-accessibility-motion-01, STD-accessibility-motion-02, STD-accessibility-motion-03, STD-accessibility-motion-04, STD-accessibility-motion-05, STD-accessibility-motion-06, STD-accessibility-motion-07, STD-accessibility-motion-08, STD-accessibility-motion-09, STD-accessibility-motion-10, STD-accessibility-motion-11, STD-accessibility-motion-12, STD-accessibility-motion-13, STD-accessibility-motion-15, STD-accessibility-motion-16, STD-accessibility-motion-17, STD-accessibility-motion-18, STD-accessibility-motion-20, STD-accessibility-motion-23, STD-accessibility-motion-24, STD-accessibility-motion-25, STD-accessibility-motion-26, STD-accessibility-motion-27, STD-components-toasts-drawers-02, STD-components-toasts-drawers-03, STD-components-toasts-drawers-04, STD-components-toasts-drawers-05, STD-components-toasts-drawers-07, STD-components-toasts-drawers-08, STD-components-toasts-drawers-10, STD-components-toasts-drawers-11, STD-components-toasts-drawers-12, STD-components-toasts-drawers-13, STD-components-toasts-drawers-14, STD-components-toasts-drawers-15, STD-components-toasts-drawers-16, STD-components-toasts-drawers-17, STD-components-toasts-drawers-18, STD-components-toasts-drawers-19, STD-components-toasts-drawers-20, STD-components-toasts-drawers-21, STD-components-toasts-drawers-22, STD-components-toasts-drawers-23, STD-components-toasts-drawers-24, STD-components-toasts-drawers-25, STD-components-toasts-drawers-26, STD-components-toasts-drawers-27, STD-components-toasts-drawers-28, STD-components-toasts-drawers-29, STD-components-toasts-drawers-30, STD-components-toasts-drawers-33, STD-components-toasts-drawers-34, STD-components-toasts-drawers-35, STD-components-toasts-drawers-37, STD-components-toasts-drawers-38, STD-components-toasts-drawers-39, STD-components-toasts-drawers-40, STD-components-toasts-drawers-44, STD-components-toasts-drawers-45, STD-components-toasts-drawers-48, STD-components-toasts-drawers-59, STD-components-toasts-drawers-60, STD-components-toasts-drawers-65, STD-components-toasts-drawers-72, STD-components-toasts-drawers-77, STD-components-toasts-drawers-78, STD-mobile-touch-02, STD-mobile-touch-03, STD-mobile-touch-05, STD-mobile-touch-06, STD-mobile-touch-07, STD-mobile-touch-08, STD-mobile-touch-09, STD-mobile-touch-10, STD-mobile-touch-11, STD-mobile-touch-13, STD-mobile-touch-14, STD-mobile-touch-15, STD-mobile-touch-16, STD-mobile-touch-17, STD-mobile-touch-18, STD-mobile-touch-19, STD-mobile-touch-20, STD-mobile-touch-21, STD-mobile-touch-24, STD-mobile-touch-28, STD-mobile-touch-30, STD-mobile-touch-33, STD-mobile-touch-34, STD-mobile-touch-35, STD-mobile-touch-36, STD-mobile-touch-37, STD-mobile-touch-38, STD-mobile-touch-39, STD-mobile-touch-41, STD-mobile-touch-42, STD-mobile-touch-44, STD-mobile-touch-48, STD-mobile-touch-51, STD-mobile-touch-60, STD-mobile-touch-61, STD-mobile-touch-62, STD-mobile-touch-67, STD-mobile-touch-70, STD-visual-details-01, STD-visual-details-02, STD-visual-details-03, STD-visual-details-04, STD-visual-details-05, STD-visual-details-06, STD-visual-details-07, STD-visual-details-08, STD-visual-details-09, STD-visual-details-10, STD-visual-details-11, STD-visual-details-13, STD-visual-details-14, STD-visual-details-15, STD-visual-details-16, STD-visual-details-17, STD-visual-details-18, STD-visual-details-19, STD-visual-details-20, STD-visual-details-21, STD-visual-details-24, STD-visual-details-25, STD-visual-details-26, STD-visual-details-27, STD-visual-details-28, STD-visual-details-29, STD-visual-details-30, STD-visual-details-31, STD-visual-details-32, STD-visual-details-33, STD-visual-details-34, STD-visual-details-35, STD-visual-details-36, STD-visual-details-37, STD-visual-details-38, STD-visual-details-39, STD-visual-details-40, STD-visual-details-41, STD-visual-details-42, STD-visual-details-43, STD-visual-details-44, STD-visual-details-45, STD-visual-details-46, STD-visual-details-47, STD-visual-details-48, STD-visual-details-49, STD-visual-details-50, STD-visual-details-51, STD-visual-details-55, STD-visual-details-56, STD-visual-details-57, STD-visual-details-59, STD-visual-details-61, STD-visual-details-62, STD-visual-details-64, STD-process-review-taste-01, STD-process-review-taste-02, STD-process-review-taste-03, STD-process-review-taste-04, STD-process-review-taste-05, STD-process-review-taste-06, STD-process-review-taste-07, STD-process-review-taste-08, STD-process-review-taste-09, STD-process-review-taste-10, STD-process-review-taste-11, STD-process-review-taste-12, STD-process-review-taste-13, STD-process-review-taste-14, STD-process-review-taste-15, STD-process-review-taste-16, STD-process-review-taste-17, STD-process-review-taste-18, STD-process-review-taste-19, STD-process-review-taste-20, STD-process-review-taste-21, STD-process-review-taste-22, STD-process-review-taste-23, STD-process-review-taste-24, STD-process-review-taste-25, STD-process-review-taste-26, STD-process-review-taste-27, STD-process-review-taste-28, STD-process-review-taste-29, STD-process-review-taste-30, STD-process-review-taste-31, STD-process-review-taste-32, STD-process-review-taste-33, STD-process-review-taste-34, STD-process-review-taste-35, STD-process-review-taste-36, STD-process-review-taste-37, STD-process-review-taste-38, STD-process-review-taste-39, STD-process-review-taste-40, STD-process-review-taste-41, STD-process-review-taste-42, STD-process-review-taste-43, STD-process-review-taste-44, STD-process-review-taste-45, STD-process-review-taste-46, STD-process-review-taste-47, STD-process-review-taste-48, STD-process-review-taste-49, STD-process-review-taste-50, STD-process-review-taste-51, STD-process-review-taste-52, STD-process-review-taste-53, STD-process-review-taste-54, STD-process-review-taste-55, STD-process-review-taste-56, STD-process-review-taste-57, STD-process-review-taste-58, STD-process-review-taste-59, STD-process-review-taste-60, STD-process-review-taste-62, STD-process-review-taste-63, STD-process-review-taste-64, STD-process-review-taste-65, STD-process-review-taste-66, STD-process-review-taste-67, STD-swift-01, STD-swift-02, STD-swift-03, STD-swift-04, STD-swift-05, STD-swift-06, STD-swift-07, STD-swift-08, STD-swift-09, STD-swift-10, STD-swift-11, STD-swift-12, STD-swift-13, STD-swift-14, STD-swift-15, STD-swift-16, STD-swift-17, STD-swift-18, STD-swift-19, STD-swift-20, STD-swift-21, STD-swift-22, STD-swift-23, STD-swift-24, STD-swift-25, STD-swift-26, STD-swift-27, STD-swift-28, STD-swift-29, STD-swift-30, STD-swift-31, STD-swift-32, STD-swift-33, STD-swift-34, STD-swift-35, STD-swift-36, STD-swift-37, STD-swift-38, STD-swift-39, STD-swift-40, STD-swift-41, STD-swift-42, STD-swift-43, STD-swift-44, STD-swift-45, STD-swift-46, STD-swift-47, STD-swift-48, STD-swift-49, STD-swift-50, STD-swift-51, STD-swift-52, STD-swift-53, STD-swift-54, STD-swift-55, STD-swift-56, STD-swift-57, STD-swift-58, STD-swift-59, STD-swift-60, STD-swift-61, STD-swift-62, STD-swift-63, STD-swift-64, STD-swift-65, STD-swift-66, STD-swift-67, STD-swift-68, STD-swift-69, STD-swift-70, STD-swift-71, STD-swift-72, STD-swift-73, STD-swift-74, STD-swift-75, STD-swift-76, STD-swift-77, STD-swift-78, STD-swift-79, STD-swift-80, STD-swift-81, STD-swift-82, STD-swift-83, STD-swift-84, STD-swift-85, STD-swift-86, STD-swift-87, STD-swift-88, STD-swift-89, STD-swift-90, STD-swift-91, STD-swift-92, STD-swift-93, STD-swift-94, STD-swift-95, STD-swift-96, STD-swift-97, STD-swift-98, STD-swift-99, STD-swift-100, STD-swift-101, STD-swift-102, STD-swift-103, STD-swift-104, STD-swift-105, STD-swift-106, STD-swift-107, STD-swift-108, STD-swift-109, STD-swift-110, STD-swift-111, STD-swift-112, STD-swift-113</details>
- STD-when-to-animate-01: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-03: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-04: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-05: motion.duration.instant = 0ms
- STD-when-to-animate-06: followed; it sets no values (DESIGN.md and review carry it)
- STD-when-to-animate-07: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-08: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-09: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-10: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-11: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-13: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-14: followed; it sets no values (DESIGN.md and review carry it)
- STD-when-to-animate-15: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-16: followed; it sets no values
- STD-when-to-animate-17: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-20: followed; it sets no values (DESIGN.md carries it)
- STD-when-to-animate-22: followed; it sets no values
- STD-easing-duration-01: motion.easing.linear = [0, 0, 1, 1]
- STD-easing-duration-01: motion.easing.hover = [0.25, 0.1, 0.25, 1]
- STD-easing-duration-02: motion.easing.enter = [0.23, 1, 0.32, 1]
- STD-easing-duration-02: motion.easing.exit = [0.23, 1, 0.32, 1]
- STD-easing-duration-02: motion.easing.standard = [0.77, 0, 0.175, 1]
- STD-easing-duration-03: followed; it sets no values (DESIGN.md and review carry it)
- STD-easing-duration-06: followed; it sets no values (DESIGN.md and review carry it)
- STD-easing-duration-07: motion.duration.micro = 100ms
- STD-easing-duration-07: motion.duration.short = 150ms
- STD-easing-duration-07: motion.duration.medium = 200ms
- STD-easing-duration-07: motion.duration.long = 250ms
- STD-easing-duration-09: followed; it sets no values (DESIGN.md carries it)
- STD-easing-duration-10: followed; it sets no values (DESIGN.md carries it)
- STD-easing-duration-11: followed; it sets no values (DESIGN.md carries it)
- STD-easing-duration-12: followed; it sets no values (DESIGN.md carries it)
- STD-easing-duration-13: followed; it sets no values (DESIGN.md carries it)
- STD-easing-duration-15: followed; it sets no values (DESIGN.md carries it)
- STD-easing-duration-17: followed; it sets no values (DESIGN.md carries it)
- STD-easing-duration-19: followed; it sets no values
- STD-enter-exit-origin-01: motion.scale.enter = 0.95
- STD-enter-exit-origin-02: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-03: followed; it sets no values (DESIGN.md and review carry it)
- STD-enter-exit-origin-04: followed; it sets no values (DESIGN.md and review carry it)
- STD-enter-exit-origin-06: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-08: motion.duration.medium = 200ms
- STD-enter-exit-origin-08: motion.scale.enter = 0.95
- STD-enter-exit-origin-09: motion.duration.tooltip = 125ms
- STD-enter-exit-origin-09: motion.scale.enter-tooltip = 0.97
- STD-enter-exit-origin-10: motion.duration.instant = 0ms
- STD-enter-exit-origin-11: motion.duration.modal = 250ms
- STD-enter-exit-origin-11: motion.scale.enter-modal = 0.96
- STD-enter-exit-origin-12: motion.duration.modal = 250ms
- STD-enter-exit-origin-13: motion.duration.stagger = 50ms
- STD-enter-exit-origin-16: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-17: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-21: followed; it sets no values (DESIGN.md and review carry it)
- STD-enter-exit-origin-23: motion.duration.medium = 200ms
- STD-enter-exit-origin-24: followed; it sets no values (DESIGN.md and review carry it)
- STD-enter-exit-origin-25: followed; it sets no values (DESIGN.md and review carry it)
- STD-enter-exit-origin-26: motion.duration.reveal = 600ms
- STD-enter-exit-origin-27: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-28: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-29: motion.blur.crossfade = 2px
- STD-enter-exit-origin-30: followed; it sets no values (DESIGN.md and review carry it)
- STD-enter-exit-origin-31: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-33: followed; it sets no values (DESIGN.md and review carry it)
- STD-enter-exit-origin-34: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-35: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-37: followed; it sets no values
- STD-enter-exit-origin-38: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-39: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-40: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-41: motion.easing.drawer = [0.32, 0.72, 0, 1]
- STD-enter-exit-origin-41: motion.duration.drawer = 500ms
- STD-enter-exit-origin-42: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-43: followed; it sets no values (DESIGN.md carries it)
- STD-enter-exit-origin-44: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-01: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-02: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-04: motion.spring.spatial.dampingRatio = 1.0
- STD-springs-gestures-04: motion.spring.spatial.stiffness = 246.7
- STD-springs-gestures-05: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-06: motion.spring.momentum = {"dampingRatio": 0.8, "stiffness": 246.7, "mass": 1}
- STD-springs-gestures-07: followed; it sets no values (DESIGN.md and review carry it)
- STD-springs-gestures-08: motion.spring.sheet = {"dampingRatio": 0.8, "stiffness": 438.6, "mass": 1}
- STD-springs-gestures-09: motion.spring.rotation = {"dampingRatio": 0.8, "stiffness": 246.7, "mass": 1}
- STD-springs-gestures-10: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-11: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-12: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-13: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-14: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-15: followed; it sets no values (DESIGN.md and review carry it)
- STD-springs-gestures-16: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-17: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-18: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-19: motion.gesture.deceleration-rate = 0.998
- STD-springs-gestures-20: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-21: motion.gesture.dismiss-velocity = 0.11
- STD-springs-gestures-22: motion.gesture.sheet-dismiss-fraction = 0.4
- STD-springs-gestures-23: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-24: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-25: motion.gesture.rubberband-constant = 0.55
- STD-springs-gestures-26: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-28: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-30: motion.gesture.direction-threshold = 10px
- STD-springs-gestures-34: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-39: followed; it sets no values (DESIGN.md and review carry it)
- STD-springs-gestures-41: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-42: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-45: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-59: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-60: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-61: followed; it sets no values (DESIGN.md carries it)
- STD-springs-gestures-63: followed; it sets no values (DESIGN.md carries it)
- STD-performance-properties-01: followed; it sets no values (DESIGN.md and review carry it)
- STD-performance-properties-02: followed; it sets no values (DESIGN.md carries it)
- STD-performance-properties-06: followed; it sets no values (DESIGN.md and review carry it)
- STD-performance-properties-09: followed; it sets no values (DESIGN.md and review carry it)
- STD-performance-properties-10: followed; it sets no values (DESIGN.md and review carry it)
- STD-performance-properties-11: followed; it sets no values (DESIGN.md and review carry it)
- STD-performance-properties-12: followed; it sets no values (DESIGN.md carries it)
- STD-performance-properties-13: followed; it sets no values (DESIGN.md carries it)
- STD-performance-properties-14: followed; it sets no values (DESIGN.md carries it)
- STD-performance-properties-15: followed; it sets no values (DESIGN.md carries it)
- STD-performance-properties-16: followed; it sets no values (DESIGN.md carries it)
- STD-performance-properties-17: followed; it sets no values (DESIGN.md carries it)
- STD-performance-properties-18: followed; it sets no values (DESIGN.md and review carry it)
- STD-performance-properties-19: followed; it sets no values (DESIGN.md and review carry it)
- STD-performance-properties-20: followed; it sets no values (DESIGN.md and review carry it)
- STD-performance-properties-24: followed; it sets no values (DESIGN.md carries it)
- STD-performance-properties-25: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-01: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-02: raw.reducedMotion = "replace"
- STD-accessibility-motion-02: motion.duration.reduced-fade = 200ms
- STD-accessibility-motion-02: reduced:motion.transition.enter = {"duration": "{motion.duration.reduced-fade}", "delay": {"value": 0, "unit": "ms"}, "timingFunction": [0.25, 0.1, 0.25, 1]}
- STD-accessibility-motion-02: reduced:motion.transition.exit = {"duration": "{motion.duration.reduced-fade}", "delay": {"value": 0, "unit": "ms"}, "timingFunction": [0.25, 0.1, 0.25, 1]}
- STD-accessibility-motion-02: reduced:motion.transition.expand = {"duration": "{motion.duration.reduced-fade}", "delay": {"value": 0, "unit": "ms"}, "timingFunction": [0.25, 0.1, 0.25, 1]}
- STD-accessibility-motion-03: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-04: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-05: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-06: followed; it sets no values
- STD-accessibility-motion-07: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-08: followed; it sets no values (DESIGN.md and review carry it)
- STD-accessibility-motion-09: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-10: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-11: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-12: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-13: followed; it sets no values (DESIGN.md and review carry it)
- STD-accessibility-motion-15: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-16: followed; it sets no values (DESIGN.md and review carry it)
- STD-accessibility-motion-17: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-18: followed; it sets no values
- STD-accessibility-motion-20: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-23: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-24: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-25: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-26: followed; it sets no values (DESIGN.md carries it)
- STD-accessibility-motion-27: followed; it sets no values (DESIGN.md and review carry it)
- STD-components-toasts-drawers-02: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-03: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-04: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-05: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-07: motion.duration.toast = 400ms
- STD-components-toasts-drawers-07: motion.easing.toast = [0.25, 0.1, 0.25, 1]
- STD-components-toasts-drawers-08: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-10: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-11: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-12: component.toast.gap = 14px
- STD-components-toasts-drawers-13: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-14: component.toast.visible = 3
- STD-components-toasts-drawers-15: component.toast.duration = 4000ms
- STD-components-toasts-drawers-16: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-17: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-18: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-19: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-20: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-21: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-22: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-23: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-24: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-25: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-26: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-27: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-28: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-29: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-30: component.toast.offset.desktop = 32px
- STD-components-toasts-drawers-30: component.toast.offset.mobile = 16px
- STD-components-toasts-drawers-33: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-34: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-35: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-37: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-38: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-39: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-40: motion.easing.drawer = [0.32, 0.72, 0, 1]
- STD-components-toasts-drawers-44: motion.gesture.drag-lock-after-scroll = 100ms
- STD-components-toasts-drawers-45: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-48: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-59: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-60: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-65: followed; it sets no values
- STD-components-toasts-drawers-72: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-77: followed; it sets no values (DESIGN.md carries it)
- STD-components-toasts-drawers-78: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-02: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-03: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-05: motion.scale.press = 0.97
- STD-mobile-touch-05: motion.duration.micro = 100ms
- STD-mobile-touch-06: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-07: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-08: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-09: size.target.touch = 44px
- STD-mobile-touch-09: size.target.min = 44px
- STD-mobile-touch-10: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-11: font.size.input = 16px
- STD-mobile-touch-13: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-14: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-15: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-16: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-17: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-18: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-19: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-20: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-21: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-24: followed; it sets no values
- STD-mobile-touch-28: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-30: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-33: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-34: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-35: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-36: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-37: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-38: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-39: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-41: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-42: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-44: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-48: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-51: motion.spring.spatial.dampingRatio = 1.0
- STD-mobile-touch-60: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-61: followed; it sets no values (DESIGN.md and review carry it)
- STD-mobile-touch-62: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-67: followed; it sets no values (DESIGN.md carries it)
- STD-mobile-touch-70: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-01: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-02: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-03: followed; it sets no values (DESIGN.md and review carry it)
- STD-visual-details-04: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-05: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-06: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-07: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-08: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-09: followed; it sets no values (DESIGN.md and review carry it)
- STD-visual-details-10: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-11: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-13: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-14: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-15: followed; it sets no values (DESIGN.md and review carry it)
- STD-visual-details-16: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-17: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-18: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-19: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-20: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-21: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-24: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-25: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-26: followed; it sets no values (DESIGN.md and review carry it)
- STD-visual-details-27: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-28: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-29: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-30: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-31: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-32: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-33: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-34: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-35: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-36: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-37: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-38: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-39: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-40: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-41: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-42: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-43: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-44: followed; it sets no values
- STD-visual-details-45: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-46: followed; it sets no values
- STD-visual-details-47: followed; it sets no values
- STD-visual-details-48: followed; it sets no values
- STD-visual-details-49: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-50: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-51: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-55: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-56: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-57: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-59: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-61: followed; it sets no values (DESIGN.md carries it)
- STD-visual-details-62: followed; it sets no values (DESIGN.md and review carry it)
- STD-visual-details-64: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-01: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-02: followed; it sets no values
- STD-process-review-taste-03: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-04: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-05: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-06: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-07: followed; it sets no values
- STD-process-review-taste-08: followed; it sets no values
- STD-process-review-taste-09: followed; it sets no values
- STD-process-review-taste-10: followed; it sets no values
- STD-process-review-taste-11: followed; it sets no values
- STD-process-review-taste-12: followed; it sets no values
- STD-process-review-taste-13: followed; it sets no values
- STD-process-review-taste-14: followed; it sets no values
- STD-process-review-taste-15: followed; it sets no values
- STD-process-review-taste-16: followed; it sets no values
- STD-process-review-taste-17: followed; it sets no values
- STD-process-review-taste-18: followed; it sets no values
- STD-process-review-taste-19: followed; it sets no values
- STD-process-review-taste-20: followed; it sets no values
- STD-process-review-taste-21: followed; it sets no values
- STD-process-review-taste-22: followed; it sets no values
- STD-process-review-taste-23: followed; it sets no values
- STD-process-review-taste-24: followed; it sets no values
- STD-process-review-taste-25: followed; it sets no values
- STD-process-review-taste-26: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-27: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-28: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-29: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-30: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-31: followed; it sets no values
- STD-process-review-taste-32: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-33: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-34: followed; it sets no values
- STD-process-review-taste-35: followed; it sets no values
- STD-process-review-taste-36: followed; it sets no values (DESIGN.md carries it)
- STD-process-review-taste-37: followed; it sets no values
- STD-process-review-taste-38: followed; it sets no values
- STD-process-review-taste-39: followed; it sets no values
- STD-process-review-taste-40: followed; it sets no values (review carries it)
- STD-process-review-taste-41: followed; it sets no values (review carries it)
- STD-process-review-taste-42: followed; it sets no values
- STD-process-review-taste-43: followed; it sets no values
- STD-process-review-taste-44: followed; it sets no values
- STD-process-review-taste-45: followed; it sets no values
- STD-process-review-taste-46: followed; it sets no values
- STD-process-review-taste-47: followed; it sets no values
- STD-process-review-taste-48: followed; it sets no values
- STD-process-review-taste-49: followed; it sets no values
- STD-process-review-taste-50: followed; it sets no values
- STD-process-review-taste-51: followed; it sets no values
- STD-process-review-taste-52: followed; it sets no values
- STD-process-review-taste-53: followed; it sets no values
- STD-process-review-taste-54: followed; it sets no values
- STD-process-review-taste-55: followed; it sets no values
- STD-process-review-taste-56: followed; it sets no values
- STD-process-review-taste-57: followed; it sets no values
- STD-process-review-taste-58: followed; it sets no values
- STD-process-review-taste-59: followed; it sets no values
- STD-process-review-taste-60: followed; it sets no values
- STD-process-review-taste-62: followed; it sets no values
- STD-process-review-taste-63: followed; it sets no values
- STD-process-review-taste-64: followed; it sets no values
- STD-process-review-taste-65: followed; it sets no values
- STD-process-review-taste-66: followed; it sets no values
- STD-process-review-taste-67: followed; it sets no values (DESIGN.md carries it)
- STD-swift-01: followed; it sets no values (DESIGN.md carries it)
- STD-swift-02: followed; it sets no values (DESIGN.md carries it)
- STD-swift-03: followed; it sets no values (DESIGN.md carries it)
- STD-swift-04: followed; it sets no values
- STD-swift-05: followed; it sets no values
- STD-swift-06: followed; it sets no values
- STD-swift-07: followed; it sets no values (DESIGN.md carries it)
- STD-swift-08: followed; it sets no values
- STD-swift-09: followed; it sets no values
- STD-swift-10: followed; it sets no values
- STD-swift-11: followed; it sets no values
- STD-swift-12: followed; it sets no values
- STD-swift-13: followed; it sets no values
- STD-swift-14: followed; it sets no values
- STD-swift-15: followed; it sets no values (DESIGN.md carries it)
- STD-swift-16: followed; it sets no values (DESIGN.md carries it)
- STD-swift-17: followed; it sets no values (DESIGN.md carries it)
- STD-swift-18: followed; it sets no values (DESIGN.md carries it)
- STD-swift-19: followed; it sets no values (DESIGN.md and review carry it)
- STD-swift-20: followed; it sets no values
- STD-swift-21: followed; it sets no values
- STD-swift-22: followed; it sets no values
- STD-swift-23: followed; it sets no values
- STD-swift-24: followed; it sets no values
- STD-swift-25: followed; it sets no values
- STD-swift-26: followed; it sets no values
- STD-swift-27: followed; it sets no values
- STD-swift-28: followed; it sets no values
- STD-swift-29: followed; it sets no values
- STD-swift-30: followed; it sets no values
- STD-swift-31: followed; it sets no values
- STD-swift-32: followed; it sets no values
- STD-swift-33: followed; it sets no values
- STD-swift-34: followed; it sets no values
- STD-swift-35: followed; it sets no values (DESIGN.md carries it)
- STD-swift-36: followed; it sets no values (review carries it)
- STD-swift-37: followed; it sets no values
- STD-swift-38: followed; it sets no values
- STD-swift-39: followed; it sets no values
- STD-swift-40: followed; it sets no values
- STD-swift-41: followed; it sets no values
- STD-swift-42: followed; it sets no values
- STD-swift-43: followed; it sets no values (DESIGN.md and review carry it)
- STD-swift-44: followed; it sets no values (DESIGN.md carries it)
- STD-swift-45: followed; it sets no values (DESIGN.md carries it)
- STD-swift-46: followed; it sets no values (DESIGN.md carries it)
- STD-swift-47: followed; it sets no values
- STD-swift-48: followed; it sets no values
- STD-swift-49: followed; it sets no values
- STD-swift-50: followed; it sets no values
- STD-swift-51: followed; it sets no values
- STD-swift-52: followed; it sets no values (review carries it)
- STD-swift-53: followed; it sets no values
- STD-swift-54: followed; it sets no values
- STD-swift-55: followed; it sets no values
- STD-swift-56: followed; it sets no values
- STD-swift-57: followed; it sets no values
- STD-swift-58: followed; it sets no values
- STD-swift-59: followed; it sets no values
- STD-swift-60: followed; it sets no values (review carries it)
- STD-swift-61: followed; it sets no values
- STD-swift-62: followed; it sets no values
- STD-swift-63: followed; it sets no values
- STD-swift-64: followed; it sets no values
- STD-swift-65: followed; it sets no values
- STD-swift-66: followed; it sets no values
- STD-swift-67: followed; it sets no values
- STD-swift-68: followed; it sets no values
- STD-swift-69: followed; it sets no values (review carries it)
- STD-swift-70: followed; it sets no values
- STD-swift-71: followed; it sets no values
- STD-swift-72: followed; it sets no values
- STD-swift-73: followed; it sets no values
- STD-swift-74: followed; it sets no values
- STD-swift-75: followed; it sets no values
- STD-swift-76: followed; it sets no values
- STD-swift-77: followed; it sets no values
- STD-swift-78: followed; it sets no values
- STD-swift-79: followed; it sets no values
- STD-swift-80: followed; it sets no values
- STD-swift-81: followed; it sets no values
- STD-swift-82: followed; it sets no values
- STD-swift-83: followed; it sets no values
- STD-swift-84: followed; it sets no values
- STD-swift-85: followed; it sets no values
- STD-swift-86: followed; it sets no values
- STD-swift-87: followed; it sets no values
- STD-swift-88: followed; it sets no values (review carries it)
- STD-swift-89: followed; it sets no values
- STD-swift-90: followed; it sets no values
- STD-swift-91: followed; it sets no values
- STD-swift-92: followed; it sets no values
- STD-swift-93: followed; it sets no values
- STD-swift-94: followed; it sets no values
- STD-swift-95: followed; it sets no values
- STD-swift-96: followed; it sets no values
- STD-swift-97: followed; it sets no values (DESIGN.md and review carry it)
- STD-swift-98: followed; it sets no values
- STD-swift-99: followed; it sets no values
- STD-swift-100: followed; it sets no values
- STD-swift-101: followed; it sets no values
- STD-swift-102: followed; it sets no values
- STD-swift-103: followed; it sets no values
- STD-swift-104: followed; it sets no values
- STD-swift-105: followed; it sets no values
- STD-swift-106: followed; it sets no values
- STD-swift-107: followed; it sets no values
- STD-swift-108: followed; it sets no values
- STD-swift-109: followed; it sets no values
- STD-swift-110: followed; it sets no values
- STD-swift-111: followed; it sets no values
- STD-swift-112: followed; it sets no values
- STD-swift-113: followed; it sets no values

## D-0003 · context.product = "a snack and drinks ordering website for Maika"
- set_by: assumed · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: from the handoff brief
- previous value: ""

## D-0004 · context.purpose = "help people browse Maika snacks and drinks and place delivery or pickup orders"
- set_by: assumed · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: from the handoff brief
- previous value: ""

## D-0005 · context.goals = ["let guests place orders without signing in", "let customers manage their cart, vouchers and reviews", "let admins manage products, orders, vouchers and reviews"]
- set_by: assumed · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: from the handoff brief
- previous value: []

## D-0006 · answers.Q-scope-07 = "building"
- set_by: assumed · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: the handoff describes an in-progress team project

## D-0007 · answers.Q-aud-01 = "large"
- set_by: assumed · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: snack orders are occasional and the brief requires responsive mobile ordering
- also set: dials.density = 15 (from Q-aud-01)

## D-0008 · context.market.analogous = "Popeyes"
- set_by: reference · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: named in the handoff as ordering-flow inspiration; identity must not be copied
- previous value: ""

## D-0009 · answers.Q-aud-01 = "large"
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: D-0007 · source_ref: none
- reason: sketch: Level 0 answer
- previous value: "large"
- also set: dials.density = 15 (from Q-aud-01)

## D-0010 · context.audience = "people who use it now and then, often on a phone"
- set_by: assumed · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: sketch: plain words for Q-aud-01
- previous value: ""

## D-0011 · raw.brandColor = "#e65100"
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: sketch: Level 0 answer

## D-0012 · answers.Q-plat-01 = ["web"]
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: sketch: Level 0 answer
- also set: raw.platforms = ["web"] (from Q-plat-01)

## D-0013 · raw.stack = ["html", "css", "vanilla-js"]
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: sketch: the code stack the person named

## D-0014 · macros = ["friendly", "bold", "playful"]
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: sketch: Level 0 answer (their words: friendly, bold, energetic)
- previous value: []

## D-0015 · taste.feelWords = ["friendly", "bold", "energetic"]
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: sketch: the person's own feel words

## D-0016 · answers.Q-scope-06 = ["website:operate"]
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: sketch: Level 0 answer
- also set: context.surfaces = [{"name": "website", "mode": "Operate"}] (from Q-scope-06)
- also set: raw.productType = "work-tool" (from Q-scope-06)
- also set: raw.marketingSurfaces = false (from Q-scope-06)

## D-0017 · House standards v3 for css, html, vanilla-js, web: 0 now apply, 166 no longer apply
- set_by: standard · locked: yes · date: 2026-11-04 · supersedes: none · source_ref: standards.json v3
- reason: The platforms or the stack changed, so the house standards were re-scoped: the ones that now apply are applied and locked; the ones that no longer apply are unlocked, not reverted.
- <details><summary>166 standards</summary> STD-when-to-animate-14, STD-enter-exit-origin-25, STD-enter-exit-origin-33, STD-enter-exit-origin-34, STD-enter-exit-origin-35, STD-springs-gestures-10, STD-springs-gestures-22, STD-springs-gestures-23, STD-springs-gestures-24, STD-performance-properties-18, STD-performance-properties-19, STD-performance-properties-20, STD-accessibility-motion-03, STD-accessibility-motion-04, STD-accessibility-motion-25, STD-components-toasts-drawers-02, STD-components-toasts-drawers-04, STD-components-toasts-drawers-05, STD-components-toasts-drawers-08, STD-components-toasts-drawers-19, STD-components-toasts-drawers-20, STD-components-toasts-drawers-21, STD-components-toasts-drawers-22, STD-components-toasts-drawers-23, STD-components-toasts-drawers-24, STD-components-toasts-drawers-26, STD-components-toasts-drawers-27, STD-components-toasts-drawers-28, STD-components-toasts-drawers-35, STD-components-toasts-drawers-38, STD-components-toasts-drawers-39, STD-components-toasts-drawers-59, STD-components-toasts-drawers-60, STD-components-toasts-drawers-78, STD-mobile-touch-30, STD-mobile-touch-33, STD-mobile-touch-34, STD-mobile-touch-35, STD-mobile-touch-36, STD-mobile-touch-37, STD-mobile-touch-38, STD-mobile-touch-39, STD-mobile-touch-41, STD-mobile-touch-42, STD-mobile-touch-44, STD-mobile-touch-48, STD-mobile-touch-51, STD-mobile-touch-60, STD-mobile-touch-61, STD-mobile-touch-62, STD-mobile-touch-67, STD-visual-details-61, STD-visual-details-62, STD-swift-01, STD-swift-02, STD-swift-03, STD-swift-04, STD-swift-05, STD-swift-06, STD-swift-07, STD-swift-08, STD-swift-09, STD-swift-10, STD-swift-11, STD-swift-12, STD-swift-13, STD-swift-14, STD-swift-15, STD-swift-16, STD-swift-17, STD-swift-18, STD-swift-19, STD-swift-20, STD-swift-21, STD-swift-22, STD-swift-23, STD-swift-24, STD-swift-25, STD-swift-26, STD-swift-27, STD-swift-28, STD-swift-29, STD-swift-30, STD-swift-31, STD-swift-32, STD-swift-33, STD-swift-34, STD-swift-35, STD-swift-36, STD-swift-37, STD-swift-38, STD-swift-39, STD-swift-40, STD-swift-41, STD-swift-42, STD-swift-43, STD-swift-44, STD-swift-45, STD-swift-46, STD-swift-47, STD-swift-48, STD-swift-49, STD-swift-50, STD-swift-51, STD-swift-52, STD-swift-53, STD-swift-54, STD-swift-55, STD-swift-56, STD-swift-57, STD-swift-58, STD-swift-59, STD-swift-60, STD-swift-61, STD-swift-62, STD-swift-63, STD-swift-64, STD-swift-65, STD-swift-66, STD-swift-67, STD-swift-68, STD-swift-69, STD-swift-70, STD-swift-71, STD-swift-72, STD-swift-73, STD-swift-74, STD-swift-75, STD-swift-76, STD-swift-77, STD-swift-78, STD-swift-79, STD-swift-80, STD-swift-81, STD-swift-82, STD-swift-83, STD-swift-84, STD-swift-85, STD-swift-86, STD-swift-87, STD-swift-88, STD-swift-89, STD-swift-90, STD-swift-91, STD-swift-92, STD-swift-93, STD-swift-94, STD-swift-95, STD-swift-96, STD-swift-97, STD-swift-98, STD-swift-99, STD-swift-100, STD-swift-101, STD-swift-102, STD-swift-103, STD-swift-104, STD-swift-105, STD-swift-106, STD-swift-107, STD-swift-108, STD-swift-109, STD-swift-110, STD-swift-111, STD-swift-112, STD-swift-113</details>
- STD-when-to-animate-14: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-enter-exit-origin-25: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-enter-exit-origin-33: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-enter-exit-origin-34: no longer applies to your platforms (react-native only); its values stay, unlocked
- STD-enter-exit-origin-35: no longer applies to your platforms (react-native only); its values stay, unlocked
- STD-springs-gestures-10: no longer applies to your platforms (react-native only); its values stay, unlocked
- STD-springs-gestures-22: no longer applies to your platforms (react-native only); its values stay, unlocked
- STD-springs-gestures-23: no longer applies to your platforms (react-native only); its values stay, unlocked
- STD-springs-gestures-24: no longer applies to your platforms (react only); its values stay, unlocked
- STD-performance-properties-18: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-performance-properties-19: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-performance-properties-20: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-accessibility-motion-03: no longer applies to your platforms (react, react-native only); its values stay, unlocked
- STD-accessibility-motion-04: no longer applies to your platforms (react-native only); its values stay, unlocked
- STD-accessibility-motion-25: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-02: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-04: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-05: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-08: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-components-toasts-drawers-19: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-20: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-21: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-22: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-23: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-24: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-26: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-27: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-28: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-35: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-38: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-39: no longer applies to your platforms (react only); its values stay, unlocked
- STD-components-toasts-drawers-59: no longer applies to your platforms (react-native only); its values stay, unlocked
- STD-components-toasts-drawers-60: no longer applies to your platforms (react-native, android, ios only); its values stay, unlocked
- STD-components-toasts-drawers-78: no longer applies to your platforms (react only); its values stay, unlocked
- STD-mobile-touch-30: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-33: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-34: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-35: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-36: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-37: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-38: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-39: no longer applies to your platforms (react-native, ios only); its values stay, unlocked
- STD-mobile-touch-41: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-42: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-44: no longer applies to your platforms (react-native, ios only); its values stay, unlocked
- STD-mobile-touch-48: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-51: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-60: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-61: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-62: no longer applies to your platforms (react-native, ios, android only); its values stay, unlocked
- STD-mobile-touch-67: no longer applies to your platforms (react-native, android only); its values stay, unlocked
- STD-visual-details-61: no longer applies to your platforms (react only); its values stay, unlocked
- STD-visual-details-62: no longer applies to your platforms (react only); its values stay, unlocked
- STD-swift-01: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-02: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-03: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-04: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-05: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-06: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-07: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-08: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-09: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-10: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-11: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-12: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-13: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-14: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-15: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-16: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-17: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-18: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-19: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-20: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-21: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-22: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-23: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-24: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-25: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-26: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-27: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-28: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-29: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-30: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-31: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-32: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-33: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-34: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-35: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-36: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-37: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-38: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-39: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-40: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-41: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-42: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-43: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-44: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-45: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-46: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-47: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-48: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-49: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-50: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-51: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-52: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-53: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-54: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-55: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-56: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-57: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-58: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-59: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-60: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-61: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-62: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-63: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-64: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-65: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-66: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-67: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-68: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-69: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-70: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-71: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-72: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-73: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-74: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-75: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-76: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-77: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-78: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-79: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-80: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-81: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-82: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-83: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-84: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-85: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-86: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-87: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-88: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-89: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-90: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-91: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-92: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-93: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-94: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-95: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-96: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-97: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-98: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-99: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-100: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-101: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-102: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-103: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-104: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-105: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-106: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-107: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-108: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-109: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-110: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-111: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-112: no longer applies to your platforms (ios, swift only); its values stay, unlocked
- STD-swift-113: no longer applies to your platforms (ios, swift only); its values stay, unlocked

## D-0018 · overrides.light:color.surface.base = {"colorSpace": "srgb", "components": [0.9922, 0.9843, 0.9686], "hex": "#fdfbf7"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: the Maika palette in the handoff brief

## D-0019 · overrides.light:color.surface.nav = {"colorSpace": "srgb", "components": [0.9922, 0.9843, 0.9686], "hex": "#fdfbf7"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: the Maika palette in the handoff brief

## D-0020 · overrides.light:color.text.primary = {"colorSpace": "srgb", "components": [0.1765, 0.1765, 0.1765], "hex": "#2d2d2d"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: the Maika palette in the handoff brief

## D-0021 · overrides.light:color.border.default = {"colorSpace": "srgb", "components": [0.9176, 0.8667, 0.7882], "hex": "#eaddc9"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: the Maika palette in the handoff brief

## D-0022 · overrides.color.brand.secondary = {"colorSpace": "srgb", "components": [1.0, 0.6549, 0.149], "hex": "#ffa726"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: the Maika palette in the handoff brief
- new color token in primitives.tokens.json

## D-0023 · answers.Q-aud-02 = "consumer"
- set_by: research · locked: no · date: 2026-11-04 · supersedes: none · source_ref: research/users.json
- reason: user research (F1, F2, F4): an everyday consumer product
- also set: raw.domain = "consumer" (from Q-aud-02)

## D-0024 · profile.library = "declined"
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: the owner chose to build the food UI from scratch

## D-0025 · overrides.size.content.max = {"value": 1312, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: maximum width for Maika storefront and admin pages
- new dimension token in semantic.tokens.json

## D-0026 · overrides.size.dialog.product.max = {"value": 832, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: maximum width for the product detail dialog
- new dimension token in semantic.tokens.json

## D-0027 · overrides.size.dialog.form.max = {"value": 480, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: maximum width for compact confirmation and form dialogs
- new dimension token in semantic.tokens.json

## D-0028 · overrides.size.dialog.max-block = {"value": 896, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: maximum dialog height before internal scrolling
- new dimension token in semantic.tokens.json

## D-0029 · overrides.size.auth.max = {"value": 544, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: comfortable reading width for the account form
- new dimension token in semantic.tokens.json

## D-0030 · overrides.size.review.list.max = {"value": 320, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: limit the review list height inside the product dialog
- new dimension token in semantic.tokens.json

## D-0031 · overrides.size.toast.max = {"value": 384, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: keep confirmation messages readable
- new dimension token in semantic.tokens.json

## D-0032 · overrides.size.cart.column.min = {"value": 320, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: minimum checkout column width before stacking
- new dimension token in semantic.tokens.json

## D-0033 · overrides.size.detail.image.max = {"value": 288, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: bound the product image in a narrow dialog
- new dimension token in semantic.tokens.json

## D-0034 · overrides.size.quantity.field = {"value": 80, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: comfortable width for a quantity input
- new dimension token in semantic.tokens.json

## D-0035 · overrides.size.table.product.min = {"value": 208, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: keep product table names legible
- new dimension token in semantic.tokens.json

## D-0036 · overrides.size.status.max = {"value": 192, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: allow order status labels to fit
- new dimension token in semantic.tokens.json

## D-0037 · overrides.size.preview.max = {"value": 352, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: bound the uploaded image preview
- new dimension token in semantic.tokens.json

## D-0038 · overrides.size.admin.sidebar.min = {"value": 192, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: minimum width for management navigation
- new dimension token in semantic.tokens.json

## D-0039 · overrides.size.admin.sidebar.max = {"value": 240, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: maximum width for management navigation
- new dimension token in semantic.tokens.json

## D-0040 · overrides.size.product.mobile.image.min = {"value": 112, "unit": "px"}
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: keep menu photography visible beside mobile product details
- new dimension token in semantic.tokens.json

## D-0041 · override STD-visual-details-24 (house standard)
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: D-0002 · source_ref: none
- reason: Chỉ giữ bảng màu sáng và bỏ chế độ tối cũ theo yêu cầu của chủ dự án.
- house standard STD-visual-details-24: Make interface colors adapt to light and dark mode: give each color role a light value and a dark value.
- why the house follows it: The source lists colors that adapt to light and dark as part of the craft that builds trust.
- unlocked: nothing (it sets no values)

## D-0042 · answers.Q-theme-01 = "light-only"
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: The owner requested a light-only Maika interface and asked to remove the previous dark palette.
- also set: raw.flags.darkMode = false (from Q-theme-01)
- also set: raw.defaultTheme = "system" (from Q-theme-01)

## D-0043 · name = "Kat"
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: The owner renamed the snack shop to Kat.
- previous value: "Maika"

## D-0044 · context.product = "a snack food ordering website for Kat"
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: D-0003 · source_ref: none
- reason: The owner confirmed the product direction is a snack shop and renamed it Kat.
- previous value: "a snack and drinks ordering website for Maika"

## D-0045 · context.purpose = "help people browse Kat's snack menu and place delivery or pickup orders"
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: D-0004 · source_ref: none
- reason: The owner confirmed the snack shop direction and the Kat name.
- previous value: "help people browse Maika snacks and drinks and place delivery or pickup orders"

## D-0046 · overrides.font.family.text = ["Be Vietnam Pro", "system-ui", "-apple-system", "Segoe UI", "Roboto", "Helvetica Neue", "Arial", "sans-serif"]
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: Use a Vietnamese-ready open sans for clarity and warmth while keeping Popeyes' restricted Chicken Sans out of Kat.

## D-0047 · answers.Q-type-02 = "no"
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: none · source_ref: none
- reason: Use the open Be Vietnam Pro font for Kat rather than a private brand font or owner-supplied asset.
- also set: hooks.H-type.status = "open-library" (from Q-type-02)
- also set: raw.fontLicence = {"web": false, "app": false, "selfHost": false} (from Q-type-02)

## D-0048 · context.goals = ["let customers browse and build a cart as guests, then sign in before checkout with account details prefilled", "let customers manage their cart, vouchers and reviews", "let admins manage products, orders, vouchers and reviews"]
- set_by: chosen · locked: no · date: 2026-11-04 · supersedes: D-0005 · source_ref: none
- reason: The evaluation record requires sign-in before checkout; keep guest browsing and cart access.
- previous value: ["let guests place orders without signing in", "let customers manage their cart, vouchers and reviews", "let admins manage products, orders, vouchers and reviews"]

## D-0049 · raw.brandColor = "#8C2224"
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: D-0011 · source_ref: none
- reason: Use the original Maika burgundy palette as requested: #8C2224 for Kat primary brand and actions.
- previous value: "#e65100"

## D-0050 · overrides.color.accent.light.10 = {"colorSpace": "srgb", "components": [0.4314, 0.1059, 0.1098], "hex": "#6e1b1c"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: none · source_ref: none
- reason: Use the original Maika palette requested by the owner.

## D-0051 · overrides.color.accent.light.11 = {"colorSpace": "srgb", "components": [0.549, 0.1333, 0.1412], "hex": "#8c2224"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: none · source_ref: none
- reason: Use the original Maika palette requested by the owner.

## D-0052 · overrides.color.neutral.light.4 = {"colorSpace": "srgb", "components": [0.898, 0.898, 0.898], "hex": "#e5e5e5"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: none · source_ref: none
- reason: Use the original Maika palette requested by the owner.

## D-0053 · overrides.light:color.surface.base = {"colorSpace": "srgb", "components": [1.0, 1.0, 1.0], "hex": "#ffffff"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: D-0018 · source_ref: none
- reason: Use the original Maika palette requested by the owner.
- previous value: {"colorSpace": "srgb", "components": [0.9922, 0.9843, 0.9686], "hex": "#fdfbf7"}

## D-0054 · overrides.light:color.surface.nav = {"colorSpace": "srgb", "components": [1.0, 1.0, 1.0], "hex": "#ffffff"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: D-0019 · source_ref: none
- reason: Use the original Maika palette requested by the owner.
- previous value: {"colorSpace": "srgb", "components": [0.9922, 0.9843, 0.9686], "hex": "#fdfbf7"}

## D-0055 · overrides.light:color.surface.sunken = {"colorSpace": "srgb", "components": [0.9608, 0.9608, 0.9608], "hex": "#f5f5f5"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: none · source_ref: none
- reason: Use the original Maika palette requested by the owner.

## D-0056 · overrides.light:color.text.primary = {"colorSpace": "srgb", "components": [0.1451, 0.1451, 0.1451], "hex": "#252525"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: D-0020 · source_ref: none
- reason: Use the original Maika palette requested by the owner.
- previous value: {"colorSpace": "srgb", "components": [0.1765, 0.1765, 0.1765], "hex": "#2d2d2d"}

## D-0057 · overrides.light:color.text.heading = {"colorSpace": "srgb", "components": [0.0667, 0.0667, 0.0667], "hex": "#111111"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: none · source_ref: none
- reason: Use the original Maika palette requested by the owner.
- new color token in semantic.color.light.tokens.json

## D-0058 · overrides.light:color.text.secondary = {"colorSpace": "srgb", "components": [0.4, 0.4, 0.4], "hex": "#666666"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: none · source_ref: none
- reason: Use the original Maika palette requested by the owner.

## D-0059 · overrides.light:color.text.tertiary = {"colorSpace": "srgb", "components": [0.4, 0.4, 0.4], "hex": "#666666"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: none · source_ref: none
- reason: Use the original Maika palette requested by the owner.

## D-0060 · overrides.light:color.text.on-brand = {"colorSpace": "srgb", "components": [0.8784, 0.8784, 0.8784], "hex": "#e0e0e0"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: none · source_ref: none
- reason: Use the original Maika palette requested by the owner.

## D-0061 · overrides.light:color.border.default = {"colorSpace": "srgb", "components": [0.898, 0.898, 0.898], "hex": "#e5e5e5"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: D-0021 · source_ref: none
- reason: Use the original Maika palette requested by the owner.
- previous value: {"colorSpace": "srgb", "components": [0.9176, 0.8667, 0.7882], "hex": "#eaddc9"}

## D-0062 · overrides.light:color.border.subtle = {"colorSpace": "srgb", "components": [0.898, 0.898, 0.898], "hex": "#e5e5e5"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: none · source_ref: none
- reason: Use the original Maika palette requested by the owner.

## D-0063 · overrides.color.brand.secondary = {"colorSpace": "srgb", "components": [0.9451, 0.8157, 0.6471], "hex": "#f1d0a5"}
- set_by: chosen · locked: no · date: 2026-11-05 · supersedes: D-0022 · source_ref: none
- reason: Use the original Maika palette requested by the owner.
- previous value: {"colorSpace": "srgb", "components": [1.0, 0.6549, 0.149], "hex": "#ffa726"}
