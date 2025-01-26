# Tailwind @apply Issue within Custom Directives

This repository demonstrates a bug where Tailwind's `@apply` directive fails to function correctly when used inside a custom directive. The problem stems from the way `@apply` resolves its context within nested directives, sometimes leading to styles not being applied as expected.

## Problem

When a custom directive attempts to apply a pre-defined Tailwind utility class via `@apply`, the class might not apply or cause unexpected behavior.

## Solution

The provided solution demonstrates a workaround to correctly resolve and apply the styles from the custom directive.  This often involves explicitly defining and applying the styles or refactoring the approach to avoid the need for nested directives within @apply.