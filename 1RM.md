# Calculating 1RM Using the Epley Formula

The **Epley formula** is one of the most widely used methods in **Strength Training Analysis** for estimating an athlete's **One-Rep Max (1RM)** based on the weight lifted and the number of repetitions completed in a single set.

## Formula

\[
1RM \approx w \times \left(1 + \frac{r}{30}\right)
\]

### Variables

- **w** (*weight*) – the weight used during the set (e.g., kilograms or pounds).
- **r** (*repetitions*) – the number of completed repetitions.

## TypeScript Implementation

```typescript
/**
 * Estimates the one-repetition maximum (1RM) using the Epley formula.
 *
 * @param weight - Weight used during the set.
 * @param reps - Number of completed repetitions.
 * @returns Estimated one-repetition maximum (1RM).
 */
export const calculateEpley1RM = (
  weight: number,
  reps: number
): number => {
  return weight * (1 + reps / 30);
};
```

## Example

Given a set performed with:

- **Weight:** 100 kg
- **Repetitions:** 5

Calculation:

\[
1RM \approx 100 \times \left(1 + \frac{5}{30}\right)
= 100 \times 1.1667
= 116.7\ \text{kg}
\]

**Estimated 1RM ≈ 116.7 kg**

## Accuracy Considerations

The Epley formula provides the most reliable estimates for sets performed in the **3–10 repetition range**. Beyond this range, the influence of **muscular endurance** increases, reducing the accuracy of the estimated one-repetition maximum.

For sets exceeding **10–12 repetitions**, the calculated 1RM should be considered an approximation rather than an exact measurement of maximal strength.

## Common Use Cases

Estimated 1RM values are commonly used for:

- Programming training intensity.
- Calculating percentage-based loads (e.g., 70%, 80%, or 90% of 1RM).
- Tracking strength progress without performing maximal lifts.
- Automatically selecting training weights in strength training applications.
