# Building or reviewing a Product Overview

## First contact

When not already answered: **"Do you already have a Product Overview, or shall we create one together?"**

If yes: locate and read it; assess completeness and only ask about consequential omissions or contradictions. If no: use [the adaptable template](../templates/product-overview-v1.md) to interview the human and progressively construct the document.

The original example used 22 topic sections. **22 is not a universal requirement**: reorganize as needed while preserving coverage of the product's relevant decisions. Avoid inventing policies to populate every heading.

## What this artifact should answer

- Problem and value, actors, audience, product behavior and user journeys.
- Committed V1 scope and explicit future scope.
- Real-world constraints, observable invariants, acceptance and quality expectations.
- Accessibility, privacy, trust, rights and validation where pertinent.
- A sufficiently comprehensive source for **later** phase decomposition.

## What this artifact should NOT decide

Do not preselect database, language, architecture, queue, auth provider, API contract, deployment provider, folder layout or implementation tickets solely to fill a product description.

These may become technical-discovery questions in a later bounded phase. When the human already imposes a real nonnegotiable technical constraint, record it clearly as a **constraint**, not an unexamined solution.

## Gate

Before treating the overview as approved:
1. Explicitly separate V1 from long-term ideas.
2. Resolve material contradictions and undefined actors/user outcomes.
3. Check that validation expectations do not overpromise evidence.
4. Obtain explicit human approval.
5. Record the approved version and source path in the project's own repository.

Reference example: [Repository-to-Course Product Overview](https://github.com/h3nrzi/Repository-to-Course/blob/main/docs/product/product-overview-v1.md).
