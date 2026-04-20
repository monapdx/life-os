# re:imagined

<img src="https://raw.githubusercontent.com/monapdx/re-imagined/refs/heads/main/logo.png" width="737">

**A human-centered styling language built around visible meaning, explicit refinement, and self-normalizing structure.**

[![SPEC](https://img.shields.io/badge/SPEC-1f6feb?style=for-the-badge)](SPEC.md) [![PARSER](https://img.shields.io/badge/PARSER-1f6feb?style=for-the-badge)](https://github.com/monapdx/re-imagined/blob/main/parser-prototype.py) [![APPROACHES](https://img.shields.io/badge/APPROACHES-1f6feb?style=for-the-badge)](APPROACHES.md) [![Syntax](https://img.shields.io/badge/Syntax-1f6feb?style=for-the-badge)](#core-syntax) [![Labels](https://img.shields.io/badge/Labels-1f6feb?style=for-the-badge)](#labels) [![Rules](https://img.shields.io/badge/Rules-1f6feb?style=for-the-badge)](#rules)

## Initial Prompt:
```
How does one go about writing a new programming language, exactly?
```
## Refinement:
```
Could you make real examples of those types of decisions, but make them understandable to a non-coder (like me) by finding comparable examples if I were making an actual spoken or written language and ask me what rule I'd choose and then tell me the pros and cons
```

[Read the full conversation here](https://chatgpt.com/share/69db2cae-ab50-83e8-92b3-71ba0aa12cfa)

## 1. **Word Order (Syntax Rules)**

You’re designing a language. How should sentences be structured?

<details>
<summary>Option A</summary>

“I eat apples.”
</details>
<details>
<summary>Option B</summary>

“Apples eat I.”

</details>
<details>
<summary>Option C</summary>

“Eat I apples.”

</details>

## 2. **Do You Require Subjects? (Explicitness vs Assumption)**

Should people always say who is doing something?

<details>
<summary>Option A</summary>

“I am going to the store.”

</details>
<details>
<summary>Option B</summary>

“Going to the store.” (subject implied)

</details>

## 3. **Strict vs Flexible Meaning (Typing Systems)**

**If someone says:**

> “The idea is heavy.”

Do you allow that?

<details>
<summary>Option A</summary>

Only literal meanings allowed (“heavy” must be physical)

</details>
<details>
<summary>Option B</summary>

Metaphors allowed (“heavy” can mean emotionally serious)

</details>

## 4. **Grammar Enforcement (Errors vs Tolerance)**

**If someone says:**

> “Me go store yesterday.”

<details>
<summary>Option A</summary>

Reject it as incorrect

</details>
<details>
<summary>Option B</summary>

Accept it if meaning is clear

</details>

## 5. **Word Creation Rules (Extensibility / Abstraction)**

Can people invent new words?

**Example:**

> “unhappiness”
> “hyper-communicative”

<details>
<summary>Option A</summary>

Fixed vocabulary only

</details>
<details>
<summary>Option B</summary>

Allow combining words freely

</details>

## 6. **Ambiguity vs Precision**

**If someone says:**

> “They saw her duck.”

Do you allow ambiguity?

<details>
<summary>Option A</summary>

Every sentence must have only one meaning

</details>
<details>
<summary>Option B</summary>

Ambiguity is acceptable

</details>

## 7. **How Memory Works (Pronouns / References)**

**You say:**

> “Sarah told Jane that she was late.”

Who is “she”?

<details>
<summary>Option A</summary>

Must always be explicit

</details>
<details>
<summary>Option B</summary>

Context decides

</details>

## 8. **Error Handling (What happens when things go wrong?)**

**If someone says something nonsensical:**

> “The moon divided by banana equals sadness.”

**Do you:**

<details>
<summary>Option A</summary>

Stop the conversation immediately

</details>
<details>
<summary>Option B</summary>

Try to interpret anyway

</details>

## 9. **Formality Level (Boilerplate vs Simplicity)**

**Do people have to speak formally like:**

> “I would like to request that you pass the salt.”

**or casually:**

> “Pass the salt.”

<details>
<summary>Option A</summary>

Formal

</details>
<details>
<summary>Option B</summary>

Casual

</details>

## 10. **Rules vs Philosophy (The Deep One You Noticed)**

This is the real heart of it.

**Are you designing a language that values:**

- precision?
- beauty?
- speed?
- accessibility?
- power?
- safety?

Because you *cannot maximize all of these at once*.

---

## My Choices

1. Option A
2. Option B will always reduce confusion or remove ambiguity, but may not always be expected in informal or casual contexts. Ideally both would be tolerated.
3. Yes, it should be allowed...but it *does* benefit everyone if there is a way to indicate intended meaning.
4. This one is really tough if I were actually making a language to speak/write. My instinct is to go with option A because "Me go to store yesterday" is glaringly incorrect English. However, it may not always be practical to expect people learning as a second language to speak perfectly. **Option A** should be corect and B **should be discouraged**.
5. There should be **some rules** on the conventions for creating new words. I would argue that "unhappiness" is already an established English word with clear meaning. Something like "dishappiness" would be much stranger to encounter and is not generally used or accepted, as far as I know...I'm fine with hyper-communicative because it uses the hyphen correctly in my view of things, but we can't just join any two words by using one either. This one is very messy and complicated.
6. Honestly, the example sentence here doesn't seem ambiguous to me...it does assume the listener already understands and knows who is meant by "her" which would imply being mid-conversation. It's unlikely a sentence like this is blurted out randomly without context. I'd say it's acceptable. I'm not sure how many other meanings "They saw her duck" could have.
7. My instinct is that "her" means Jane. If it were Sarah, it would be "Sarah told Jane that she had been late. I saw **Option B** wins here.
8. Option A
9. This depends entirely on the situation, participants and social expectations. Formal and informal speech are just as valid and real as the other.
10. I would prioritize: power, accessibility and speed

---

## Overview

**re:imagined** is a tiny styling language concept that prioritizes readability over memorized positional shorthand.

[![SPEC](https://img.shields.io/badge/SPEC-1f6feb?style=for-the-badge)](SPEC.md) [![PARSER](https://img.shields.io/badge/PARSER-1f6feb?style=for-the-badge)](https://github.com/monapdx/re-imagined/blob/main/parser-prototype.py) [![APPROACHES](https://img.shields.io/badge/APPROACHES-1f6feb?style=for-the-badge)](APPROACHES.md) [![Syntax](https://img.shields.io/badge/Syntax-1f6feb?style=for-the-badge)](#core-syntax) [![Labels](https://img.shields.io/badge/Labels-1f6feb?style=for-the-badge)](#labels) [![Rules](https://img.shields.io/badge/Rules-1f6feb?style=for-the-badge)](#rules)

**Its core ideas are:**

* **labels** define meaning, not **position**
* **shorthand** should match **natural human grouping**
* **refinement** must be **explicit**
* **dead information** should never survive
* the **written form** should always reflect the **current truth**

## Core Syntax

### Declaration

```txt
padding: v 10 h 16
corner-radius: t 12 b 6
```

### Refinement

```txt
padding: v 10 h 16
^ padding: l 20
```

### Visible normalization

```txt
padding: v 10 h 16
^ padding: l 20
```

**normalizes to:**

```txt
padding: v 10 l 20 r 16
```

## Labels

### Axes

* `v` = vertical (`top + bottom`)
* `h` = horizontal (`left + right`)

### Sides

* `t` = top
* `r` = right
* `b` = bottom
* `l` = left

### Corners

* `tl` = top-left
* `tr` = top-right
* `br` = bottom-right
* `bl` = bottom-left

## Rules

### 1. Labels over position

When labels are present, order does not matter.

```txt
padding: h 16 v 10
```

**means the same thing as:**

```txt
padding: v 10 h 16
```

### 2. No overlapping definitions

A single declaration cannot define the same underlying target twice.

**Invalid:**

```txt
padding: h 16 l 20
```

because `h` already includes `l`.

### 3. Natural grouping preferred

The language prefers the shortest form that is still clear.

**Preferred:**

```txt
padding: v 10 h 16
corner-radius: t 15 b 10
```

**Valid but less preferred:**

```txt
padding: t 10 r 16 b 10 l 16
```

### 4. Refinement must be explicit

A refinement uses `^`.

```txt
padding: v 10 h 16
^ padding: l 20
```

### 5. Refinement is visible

The source should update to the normalized result rather than keep stale history.

### 6. No dead information

If a grouped value no longer contributes meaning, it disappears.

```txt
padding: v 10 h 16
^ padding: l 20 r 25
```

**becomes:**

```txt
padding: v 10 l 20 r 25
```

### 7. Simplify only when clarity is preserved

**Good simplification:**

```txt
padding: t 10 r 10 b 10 l 10
```

**becomes:**

```txt
padding: 10
```

**Good simplification:**

```txt
padding: t 10 r 16 b 10 l 16
```

**becomes:**

```txt
padding: v 10 h 16
```

**Bad simplification:**

```txt
corner-radius: t 15 b 10
```

**should **not** become:**

```txt
corner-radius: 15 10
```

because that would hide meaning behind positional convention.

### 8. No mixed units inside values

**So this is invalid:**

```
padding: v 10px h 5%
```
Because a declaration cannot mix unit systems.

### 9. Units are declared separately and persist downward

So units behave like a current measurement context for the lines that follow.

**Example:**

```
unit: px
padding: v 10 h 16
corner-radius: t 12 b 6

unit: %
width: 50
height: 25
```
**This would mean:**

the first group uses px
then unit: % changes the default for everything after it

### 10. Interpretation rule

Every numeric value after that uses the current unit unless and until another unit declaration appears.

So:

```
unit: px
padding: v 10 h 16
^ padding: l 20
```

means all those numbers are in px.

**Then if later:**

```
unit: rem
padding: 2
```

that new padding is in rem.

### 11. Unit Context

A unit declaration establishes the active numeric unit for all following numeric declarations until another unit declaration overrides it.

**Example:**

```
unit: px
padding: v 10 h 16
corner-radius: t 12 b 6
```

```
unit: rem
padding: 2
```
### Unit Rules

- Numeric declarations MUST use the current active unit.
- Mixed units within a declaration are not allowed.
- A new unit declaration replaces the previous unit context for subsequent lines.
- Refinements inherit the active unit context of their position in the document.

- Units are declared separately
- A unit declaration stays in effect until another one appears later
- That means a property and its refinements should stay within one unit context

## Example Flow

```txt
padding: v 10 h 16
^ padding: l 20
^ padding: r 25
```

**Final visible result:**

```txt
padding: v 10 l 20 r 25
```

## Design Principles

* clarity over convention
* visible meaning over positional guessing
* explicit refinement over silent override
* normalization over dead history
* simplification when it helps, not when it obscures


