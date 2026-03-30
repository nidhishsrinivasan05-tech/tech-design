# Technical Drawing Comprehensive Mastery Guide


# Table of Contents

1. [Introduction to Technical Drawing](#1-introduction-to-technical-drawing)
2. [Orthographic Projections and the Projection Cube](#2-orthographic-projections-and-the-projection-cube)
3. [Line Types and Their Applications](#3-line-types-and-their-applications)
4. [Drawing Formats and Documentation Standards](#4-drawing-formats-and-documentation-standards)
5. [Title Blocks and Drawing Identification](#5-title-blocks-and-drawing-identification)
6. [Types of Technical Drawings](#6-types-of-technical-drawings)
7. [Special Drawing Representations](#7-special-drawing-representations)
8. [Sections and Cuts](#8-sections-and-cuts)
9. [Threads and Threaded Components](#9-threads-and-threaded-components)
10. [Fastening Assemblies](#10-fastening-assemblies)
11. [Dimensioning Rules and Best Practices](#11-dimensioning-rules-and-best-practices)
12. [Cavalier and Cabinet Perspectives](#12-cavalier-and-cabinet-perspectives)
13. [Surface Intersections](#13-surface-intersections)
14. [The Technical Drawing Process](#14-the-technical-drawing-process)
15. [Assembly Plan Interpretation](#15-assembly-plan-interpretation)
16. [Standardized Fastening Elements](#16-standardized-fastening-elements)
17. [Technical Terminology and Definitions](#17-technical-terminology-and-definitions)
18. [Appendices and Reference Materials](#18-appendices-and-reference-materials)

---

# 1. Introduction to Technical Drawing

## 1.1 What is Technical Drawing?

**Technical drawing**, also known as **engineering drawing** or **industrial drawing**, is a precise graphical representation of objects, structures, and systems that conveys all the geometric, dimensional, and functional information necessary for their manufacture, inspection, and maintenance. Unlike artistic drawings or freehand sketches, technical drawings adhere to strict conventions, standards, and protocols that ensure unambiguous communication across languages, cultures, and time periods.

The fundamental principle underlying all technical drawing is **completeness without ambiguity**. Every object that can be manufactured must be represented in a way that leaves no room for misinterpretation. A single projection, view, or dimension is rarely sufficient to fully describe a three-dimensional object. Consider, for example, a simple cylindrical shaft with a keyway groove. From the front view, you might see a rectangle with parallel sides. From the top view, you would see a circle with a rectangular notch removed. Neither view alone is sufficient to manufacture the part; you need both views working together to understand the complete geometry.

### 1.1.1 The Historical Context of Technical Drawing

Technical drawing has ancient origins, with evidence of orthographic-like representations found in Egyptian architectural drawings from 2000 BCE and Roman engineering plans. However, the systematic codification of drawing conventions began in the Renaissance with figures like Leonardo da Vinci, who created remarkably detailed mechanical drawings that anticipated modern representation techniques.

The Industrial Revolution of the 18th and 19th centuries drove the need for standardized drawing practices. As manufacturing moved from individual craftspeople to interchangeable parts and assembly lines, precise communication became essential. French engineer Gaspard Monge is credited with formalizing descriptive geometry—the mathematical foundation of orthographic projection—in the late 18th century. His work laid the groundwork for the international standards we use today.

### 1.1.2 Why Multiple Views Are Necessary

**Example 1.1: The Simple L-Bracket Problem**

Consider an L-shaped bracket fabricated from a single piece of 10mm thick steel plate. The shape, when viewed from different directions, appears as follows:

```
VIEW FROM FRONT:          VIEW FROM TOP:            VIEW FROM RIGHT SIDE:
┌─────────────┐           ┌─────────────────┐       ┌───────────────┐
│             │           │                 │       │               │
│             │           │                 │       │               │
│             │           │                 │       │               │
│             │           └─────────────────┘       │               │
│             │                                     │               │
│             │                                     │               │
└─────────────┘                                     └───────────────┘
     │ 80mm                       60mm                    │ 50mm
     │                                                    │
     ▼                                                    ▼
  HEIGHT                                               DEPTH
```

**Analysis:**
- The front view shows the L-shape outline but tells us nothing about the thickness (10mm)
- The top view shows the length and width but not the height
- The right-side view shows the height and thickness but not the full width

**Conclusion:** All three views working together provide the complete dimensional information needed: 60mm × 80mm × 50mm with 10mm thickness.

**Example 1.2: The Complex Housing Problem**

Consider a pump housing with an irregular external profile and multiple internal cavities. A single view would show only one aspect of the geometry. To fully define such a part, engineers typically require:

| View | Purpose | Information Provided |
|------|---------|---------------------|
| Front view | Primary reference | Overall height, major features, mounting bosses |
| Top view | Plan reference | Overall length, width, bolt hole locations |
| Right-side view | Side reference | Depth dimensions, profile variations |
| Section A-A | Internal geometry | Internal cavities, wall thicknesses |
| Section B-B | Secondary internal | Fluid passages, internal features |
| Detail C | Local enlargement | Threaded holes, small features |

**Example 1.3: The Hidden Feature Problem**

A mechanical part has a blind hole that does not penetrate through the material. From the exterior views, you might see a circular feature but cannot determine:
- Whether it is a hole or a boss (protrusion)
- The depth of the feature
- Whether it is threaded or smooth

Only through section views can you definitively determine the internal geometry.

### 1.1.3 The Language of Technical Drawing

Technical drawing is often called "the universal language of engineering." This phrase encapsulates several important concepts:

1. **Visual Language:** Technical drawings use standardized symbols, line types, and conventions that convey meaning regardless of the reader's native language.

2. **Mathematical Precision:** Every line, curve, and dimension has a specific numerical value that can be measured, calculated, or verified.

3. **Unambiguous Communication:** The strict adherence to standards ensures that any qualified engineer, anywhere in the world, can interpret a technical drawing identically.

4. **Legal Document:** A technical drawing is a legally binding document that defines contractual obligations between designer and manufacturer.

## 1.2 The Fundamental Principles of Technical Drawing

### 1.2.1 Orthographic Projection Theory

Orthographic projection is the foundation of all technical drawing. The word "orthographic" derives from the Greek words "orthos" (straight, correct) and "graphia" (drawing, writing). In orthographic projection, the observer views the object from an infinite distance along lines that are perpendicular (orthogonal) to the projection plane. This eliminates perspective distortion, where parallel lines would appear to converge at a vanishing point.

**Mathematical Foundation:**

```
For any point P(x, y, z) in 3D space, the orthographic projection onto
the XY plane (front view) is simply P'(x, y, 0).

The projection vector is perpendicular to the projection plane:
- For the Front View (XY plane): projection along the Z-axis
- For the Top View (XZ plane): projection along the Y-axis
- For the Side View (YZ plane): projection along the X-axis
```

**Key Properties of Orthographic Projection:**

| Property | Description | Importance |
|----------|-------------|------------|
| True Shape | Circles appear as circles, parallel lines remain parallel | Enables accurate measurement |
| True Size | Distances parallel to projection plane are true size | Critical for dimensioning |
| No Distortion | Angles are preserved only in planes parallel to projection plane | Affects which views show true geometry |
| Scale Relationship | Object size relates to drawing size by a defined scale factor | Allows drawings of any size object |

### 1.2.2 The Projection Systems: First-Angle vs. Third-Angle

There are two internationally recognized systems for arranging orthographic views: **First-Angle Projection** (used primarily in Europe, Asia, and much of the world) and **Third-Angle Projection** (used primarily in the United States, Canada, and some other countries).

**First-Angle Projection Convention:**

In first-angle projection, the object is considered to be positioned between the observer and the projection plane. To obtain the top view, imagine the object rotating downward (as if folding down the top projection plane). To obtain the front view, imagine the front plane rotating backward.

```
Visual Representation of First-Angle Projection:

       Observer
          │
          ▼
    ┌─────────────┐
    │   FRONT     │  ← First projection plane (vertical)
    │   VIEW      │
    └──────┬──────┘
           │
           ▼ FOLD
    ┌─────────────┐
    │    TOP      │  ← Second projection plane (horizontal)
    │    VIEW     │     rotated DOWN from vertical
    └─────────────┘
           │
           ▼ FOLD
    ┌─────────────┐
    │   RIGHT     │  ← Third projection plane (side)
    │   VIEW      │     rotated LEFT from vertical
    └─────────────┘
```

**Third-Angle Projection Convention:**

In third-angle projection, the projection planes are positioned between the observer and the object. The top view is placed above the front view (as if the top plane folded upward), and the side view is placed to the right of the front view (as if the side plane folded to the right).

```
Visual Representation of Third-Angle Projection:

    ┌─────────────┐
    │    TOP      │  ← Top plane folded UP
    │    VIEW     │
    └──────┬──────┘
           │
    ┌──────▼──────┐
    │   FRONT     │  ← Observer views this plane
    │   VIEW      │
    └──────┬──────┘
           │
    ┌──────▼──────┐
    │   RIGHT     │  ← Side plane folded RIGHT
    │   VIEW      │
    └─────────────┘
```

**Comparison Table: First-Angle vs. Third-Angle Projection**

| Aspect | First-Angle Projection | Third-Angle Projection |
|--------|----------------------|------------------------|
| Object Position | Between observer and planes | Behind planes from observer |
| Top View Position | Below front view | Above front view |
| Right-Side View | To the left of front view | To the right of front view |
| Primary Users | Europe, Asia, ISO standard | USA, Canada, ASME standard |
| Symbol Indicator | A small circle with "A" or horizontal line below | A small cone (frustum) with "A" or horizontal line below |
| View Arrangement | Unfolded cube appears to unfold outward from front | Unfolded cube appears to unfold toward front |

**Example 1.4: First-Angle vs. Third-Angle View Arrangement**

Given a simple rectangular block with a cylindrical hole through the top, draw the front, top, and right-side views in both projection systems.

**Solution for First-Angle Projection:**

```
Standard Layout (First-Angle):

                    TOP VIEW
                    (front face projected upward,
                     rotated down)
    ┌─────────────────────────┐
    │                         │
    │                         │
    └─────────────────────────┘
              │
              │ (fold line)
              ▼
    ┌─────────┐    ┌─────────┐
    │  LEFT   │    │  FRONT  │    │  RIGHT  │
    │  SIDE   │◄───│  VIEW   │───►│  SIDE   │
    │  VIEW   │    │         │    │  VIEW   │
    └─────────┘    └─────────┘    └─────────┘
                            ▲
                            │ (fold line)
                    ┌───────────────┐
                    │     BOTTOM     │
                    │     VIEW       │
                    └───────────────┘
```

**Solution for Third-Angle Projection:**

```
Standard Layout (Third-Angle):

                    ┌───────────────┐
                    │     TOP       │
                    │     VIEW      │
                    └───────────────┘
                            ▲
                            │ (fold line)
    ┌─────────┐    ┌─────────────┐
    │  LEFT   │    │   FRONT     │    ┌─────────┐
    │  SIDE   │    │   VIEW      │    │  RIGHT  │
    │  VIEW   │    │             │    │  SIDE   │
    └─────────┘    └─────────────┘    │  VIEW   │
                            │         └────┬────┘
                            │ (fold line)  │
                            ▼              │
                    ┌───────────────┐     │
                    │   BOTTOM      │◄────┘
                    │   VIEW        │
                    └───────────────┘
```

### 1.2.3 Understanding View Correspondence

A critical skill in technical drawing is understanding how features correspond between views. Lines that are vertical in one view are vertical in adjacent views. Lines that are horizontal in one view are horizontal in adjacent views. Points that align vertically or horizontally in the drawing must maintain those relationships.

**Example 1.5: Tracing a Feature Across Views**

Consider a cast metal housing with the following features:
- A rectangular mounting pad on the top surface
- A cylindrical boss on the front face
- A clearance hole passing through the mounting pad

**Step-by-Step Analysis:**

```
Step 1: Identify the mounting pad in each view
        TOP VIEW: shows the rectangular outline of the pad
        FRONT VIEW: shows the pad as a protrusion with height
        SIDE VIEW: shows the pad depth

Step 2: Identify the boss in each view
        TOP VIEW: circular feature within or overlapping the pad
        FRONT VIEW: shows the curved profile of the cylindrical boss
        SIDE VIEW: confirms the circular nature of the boss

Step 3: Identify the hole in each view
        TOP VIEW: shows the circular cross-section of the hole
        FRONT VIEW: shows the hole opening in the pad surface
        SIDE VIEW: shows the depth of hole (may appear as hidden lines)
```

## 1.3 Common Pitfalls for Beginners

### Pitfall 1: Assuming One View is Sufficient

**What happens:** A student completes only the front view, believing it shows the object adequately.

**Why it's wrong:** As demonstrated throughout this section, a single view cannot convey three-dimensional geometry. Critical information about depth, thickness, and internal features would be missing.

**How to avoid:** Always ask yourself: "What questions would remain if I could only see this view?" If any question remains unanswered, additional views are necessary.

### Pitfall 2: Misunderstanding First vs. Third Angle

**What happens:** A student draws third-angle projections but labels the drawing as first-angle, or vice versa.

**Why it's wrong:** This fundamental error can lead to manufacturing parts that are mirror images of the intended design, causing catastrophic assembly failures.

**How to avoid:** Always identify the projection system on your drawing (ISO standard requires a symbol to be shown). When working problems, explicitly note which system you are using.

### Pitfall 3: Inconsistent Line Work

**What happens:** Lines that should align between views are slightly offset, creating a sense of "floating" features.

**Why it's wrong:** This suggests the drafter does not understand projection relationships and may have made other errors.

**How to avoid:** Use construction lines that extend beyond the final view boundaries. These guide lines should be drawn lightly and then used to verify alignment before creating final, dark lines.

## 1.4 Best Practices for Technical Drawing

1. **Plan Your Layout:** Before committing to final lines, sketch a rough layout of where each view will be placed, ensuring adequate spacing and centering on the sheet.

2. **Start with Construction Lines:** Use thin, light pencil strokes to establish the basic bounding box of each view. These can be erased later.

3. **Work Systematically:** Complete one feature at a time across all views. Do not finish the front view completely before starting other views.

4. **Maintain Consistency:** Keep your pencil sharp. Vary line darkness by pressure, not by using multiple pencils of different weights.

5. **Verify Constantly:** Compare views frequently to ensure correspondence. Use check marks or other notation to track which features have been verified.

6. **Follow Standards:** Learn and adhere to the relevant standards (ISO 128, ASME Y14.5, etc.) even when drawing by hand.

## 1.5 References and Further Reading

- **ISO 128-1:2020** — Technical drawings — General principles of representation — Part 1: Introduction and index
- **ISO 128-20:1999** — General principles of representation — Part 20: Conventions for lines on technical drawings
- **ISO 128-21:1999** — General principles of representation — Part 21: Preparation of lines by CAD systems
- **ASME Y14.5-2018** — Dimensioning and Tolerancing Principles
- **French Standard NF E04-011** — Technical drawings — Methods of projection
- **Bertoline, G.M., et al.** — *Technical Graphics Communication*, 4th Edition, McGraw-Hill Education

---

# 2. Orthographic Projections and the Projection Cube

## 2.1 The Projection Cube Concept

The **projection cube** (also called the **glass cube** or **auxiliary reference system**) is a fundamental mental model that helps visualize how orthographic views are created and arranged. Imagine your object placed inside a transparent cube, with each face of the cube representing a potential projection plane. When you project the object perpendicularly onto each cube face and then "unfold" the cube like a box, you obtain the standard arrangement of views on a drawing sheet.

### 2.1.1 Why Use a Projection Cube?

The projection cube concept serves several pedagogical and practical purposes:

1. **Visualization Aid:** It helps students understand how three-dimensional objects relate to their two-dimensional representations.

2. **View Arrangement:** It provides a logical system for arranging views on a drawing sheet.

3. **View Identification:** Each view corresponds to a specific cube face, making identification unambiguous.

4. **Completeness Check:** It reminds drafters to consider all six principal views, not just the three most common ones.

### 2.1.2 The Six Principal Views

When fully unfolded, the projection cube provides six views of the object:

| View Name | Observer Position | Projection Plane | Common Position on Drawing |
|-----------|-------------------|------------------|----------------------------|
| Front view | Looking from the front | Vertical, behind object | Center of arrangement |
| Top view | Looking from above | Horizontal, below object | Above front view |
| Bottom view | Looking from below | Horizontal, above object | Below front view |
| Right-side view | Looking from the right | Vertical, right of object | To the right of front view |
| Left-side view | Looking from the left | Vertical, left of object | To the left of front view |
| Rear view | Looking from the back | Vertical, in front of object | Varies (see below) |

**Standard Arrangements:**

For first-angle projection (ISO standard):
```
            ┌─────────────┐
            │   BOTTOM     │
            │    VIEW      │
            └─────────────┘
                    │
    ┌─────────┐     │     ┌─────────┐
    │  LEFT   │     │     │  FRONT  │     ┌─────────┐
    │  SIDE   │     │     │  VIEW   │     │  RIGHT  │
    │  VIEW   │     │     │         │     │  SIDE   │
    └─────────┘     │     └─────────┘     │  VIEW   │
                    │                     └─────────┘
                    ▼
            ┌─────────────┐
            │    TOP       │
            │    VIEW      │
            └─────────────┘
                    │
                    ▼
            ┌─────────────┐
            │   REAR      │
            │   VIEW      │
            └─────────────┘
```

For third-angle projection (ASME standard):
```
            ┌─────────────┐
            │    TOP       │
            │    VIEW      │
            └─────────────┘
                    │
    ┌─────────┐     │     ┌─────────┐
    │  LEFT   │     │     │  FRONT  │     ┌─────────┐
    │  SIDE   │     │     │  VIEW   │     │  RIGHT  │
    │  VIEW   │     │     │         │     │  SIDE   │
    └─────────┘     │     └─────────┘     │  VIEW   │
                    │                     └─────────┘
                    ▼
            ┌─────────────┐
            │   BOTTOM    │
            │    VIEW     │
            └─────────────┘
                    │
                    ▼
            ┌─────────────┐
            │   REAR      │
            │   VIEW      │
            └─────────────┘
```

### 2.1.3 Layout of Views After Unfolding the Projection Cube

Understanding the precise arrangement of views after unfolding is crucial for creating correct technical drawings. The standard relationships are:

**First-Angle Projection Layout Rules:**
1. The **right-side view** is placed to the **LEFT** of the front view
2. The **left-side view** is placed to the **RIGHT** of the front view
3. The **top view** is placed **BELOW** the front view
4. The **bottom view** is placed **ABOVE** the front view
5. The **rear view** may be placed to either extreme left or extreme right, depending on available space and drafting preference

**Third-Angle Projection Layout Rules:**
1. The **right-side view** is placed to the **RIGHT** of the front view
2. The **left-side view** is placed to the **LEFT** of the front view
3. The **top view** is placed **ABOVE** the front view
4. The **bottom view** is placed **BELOW** the front view
5. The **rear view** may be placed adjacent to the left or right views

**Example 2.1: Arranging Views for a Bracket**

Given: A mounting bracket with a triangular profile, mounting holes, and a welded reinforcement gusset.

**Step-by-Step View Arrangement:**

```
Step 1: Identify the object orientation
        - Front face is the most detailed or characteristic face
        - Select orientation that shows most features in true shape

Step 2: Draw the front view (center of layout)
        ┌──────────────────────────┐
        │                          │
        │    TRIANGULAR PROFILE    │
        │         WITH HOLES        │
        │                          │
        └──────────────────────────┘

Step 3: Project to adjacent views using fold lines
        (First-angle shown)
        
                    ┌──────────────────┐
                    │    TOP VIEW      │
                    │   (wider than    │
                    │    front)        │
                    └──────────────────┘
                            │
        ┌──────────┐        │        ┌──────────┐
        │  LEFT    │        │        │  RIGHT   │
        │  SIDE    │◄───────┴───────►│  SIDE    │
        │  VIEW    │    FRONT VIEW   │  VIEW    │
        │          │                  │          │
        └──────────┘                  └──────────┘
                            │
                    ┌──────────────────┐
                    │   BOTTOM VIEW    │
                    │                  │
                    └──────────────────┘

Step 4: Add the rear view (if required)
        Typically placed to one side, maintaining alignment
```

### 2.1.4 Fold Lines and Projection Lines

**Fold lines** (also called **folding lines** or **reference lines**) are imaginary lines that represent the edges of the projection cube after unfolding. They help maintain alignment between views and indicate the direction of projection.

**Key principles:**
- Fold lines are drawn as thin chain lines (alternating long and short dashes)
- Features on the object that align with fold lines project directly without offset
- Features offset from fold lines maintain their relative distances

**Projection lines** are light guidelines that connect corresponding features between adjacent views. They are construction aids and are typically erased before finalizing the drawing.

**Example 2.2: Using Fold Lines Correctly**

```
Drawing a cylindrical feature that is offset from center:

    FRONT VIEW                  TOP VIEW
    ┌────────────┐
    │            │────────────────────────┐
    │    ○       │    ○                    │  ← Projection lines
    │  (hole)    │     (circular profile)  │     show corresponding
    │            │────────────────────────┘     points
    └────────────┘
         │
         │ ← Feature is 15mm from left edge in front view
         │   Must be 15mm from left edge in top view
         ▼
    FOLD LINE (vertical, thin chain line)
```

## 2.2 Choosing Which Views to Draw

In practice, technical drawings rarely include all six principal views. The drafter must determine the minimum set of views that fully describes the object.

### 2.2.1 Selection Criteria

**Consider the following factors:**

1. **Complexity of the object:** More complex objects require more views
2. **Symmetry:** Symmetric parts may require only half-views
3. **Hidden features:** Sections may replace hidden lines
4. **Standard practices:** Some industries have established conventions
5. **Manufacturing needs:** Views needed for manufacturing operations

**General Guidelines:**

| Object Type | Typical Views Required |
|-------------|------------------------|
| Simple block | Front + Top (or Front + Side) |
| Cylindrical part | Front + Side (shows true circular profile) |
| Complex casting | Front + Top + Side + Sections |
| Sheet metal part | Front + Side + Detail views |
| Welded assembly | Front + Top + Isometric + Details |

### 2.2.2 Worked Example: Selecting Views for a Pump Cover

**Problem:** Select appropriate views for a pump cover shown below in isometric sketch.

**Object Description:**
- Overall dimensions: 200mm diameter × 80mm thick
- Central inlet port: 50mm diameter, through hole
- Mounting flange: 8 × 12mm slots on 160mm bolt circle
- Peripheral outlet ports: 2 × 30mm diameter, angled 45° to face
- Surface finish: 3.2 μm Ra on mating surfaces

**View Selection Analysis:**

```
Step 1: Identify the primary reference faces
        - The large circular face (200mm diameter) is the primary mating surface
        - This face should be shown as the front view

Step 2: Consider what features need to be shown
        - Circular profile: Front view shows true circular shape
        - Mounting slots: Top view shows bolt pattern and spacing
        - Port angles: Side view or section shows port orientation
        - Thickness: Side view shows 80mm dimension
        - Internal geometry: Section A-A shows inlet port and wall thickness

Step 3: Determine minimum view set
        Minimum: Front view + Top view + Section A-A
        Adequate: Front view + Top view + Side view + Section A-A
        Comprehensive: All above + Detail for mounting slots

Step 4: Layout the drawing
        
                    ┌─────────────────────┐
                    │      TOP VIEW        │
                    │   (bolt pattern)     │
                    └─────────┬───────────┘
                              │
        ┌───────────┐         │         ┌───────────┐
        │    LEFT   │         │         │   RIGHT   │
        │   SIDE    │         │         │   SIDE    │
        │   VIEW    │◄────────┴─────────►│   VIEW    │
        │           │      FRONT VIEW    │           │
        │           │                     │           │
        └───────────┘                     └───────────┘
                              │
                    ┌─────────▼───────────┐
                    │    SECTION A-A      │
                    │   (inlet detail)    │
                    └─────────────────────┘
```

**Conclusion:** This pump cover requires minimum 3 orthographic views plus 1 section to fully describe.

### 2.2.3 Example 2.3: Handling Complex Geometry

**Problem:** Draw a Y-shaped pipe fitting that connects three cylindrical branches at different angles.

**Analysis:**
```
Isometric View of Y-Fitting:

              ╱╲
             ╱  ╲
            ╱    ╲
           │      │    ← 45° branch (vertical)
           │      │
           │      │
            ╲    ╱
             ╲  ╱
              ╲╱
         ←───── Main body (horizontal) ─────→

Total length: 300mm
Main bore: 80mm diameter
Branch bore: 60mm diameter
Wall thickness: 6mm
```

**Solution Approach:**

```
Step 1: Establish principal orientation
        - Align the horizontal axis with the horizontal plane
        - The 45° branch requires special consideration

Step 2: Select views to show
        a) FRONT VIEW: Shows the Y-shape in its plane
        b) TOP VIEW: Shows the horizontal extent and centerlines
        c) SIDE VIEW: Shows the profile of the main body and branch heights
        d) SECTION: Shows wall thickness and internal bore transitions

Step 3: Handle the oblique branch
        The 45° branch cannot be shown in true projection in any 
        principal view. An auxiliary view or aligned section is needed.

Step 4: Final drawing layout
        
                    ┌──────────────────────┐
                    │      TOP VIEW         │
                    │                       │
                    └──────────┬────────────┘
                               │
        ┌───────────┐          │          ┌───────────┐
        │           │          │          │  SECTION  │
        │   SIDE    │◄─────────┴─────────►│    A-A    │
        │   VIEW    │      FRONT VIEW     │           │
        │           │                     │           │
        └───────────┘                     └───────────┘
                               │
                    ┌──────────▼────────────┐
                    │   AUXILIARY VIEW       │
                    │  (45° branch detail)   │
                    └───────────────────────┘
```

## 2.3 Auxiliary Views

Auxiliary views are additional projections used when principal views do not show features in their true shape or size. They are essential for representing oblique (non-perpendicular) surfaces accurately.

### 2.3.1 Types of Auxiliary Views

| Type | Description | When Used |
|------|-------------|----------|
| Primary auxiliary | Projected from a principal view onto a plane inclined to projection planes | Oblique surfaces |
| Secondary auxiliary | Projected from a primary auxiliary view | Complex oblique features |
|局部 auxiliary (Partial auxiliary) | Shows only the area of interest | Small oblique features |
| True-length auxiliary | Shows true length of inclined edges | Dimensioning inclined edges |

### 2.3.2 Example 2.4: Primary Auxiliary View

**Problem:** Draw an auxiliary view to show the true shape of an inclined surface on a machine housing.

**Given:**
- Inclined surface makes 30° angle with horizontal
- Surface contains a rectangular pocket
- Pocket dimensions: 40mm × 25mm

**Step-by-Step Solution:**

```
Step 1: Identify the inclined surface in the front view

    FRONT VIEW:
    ┌─────────────────────────┐
    │                         │
    │    ╱──────────────╱    │  ← Inclined surface
    │   ╱   RECTANGLE   ╱     │     (appears foreshortened)
    │  ╱    POCKET     ╱      │
    │ ╱               ╱       │
    └─────────────────────────┘
         30° angle to horizontal

Step 2: Draw the fold line (reference line) perpendicular to
        the direction of projection

    Fold line is perpendicular to the projection direction
    (typically perpendicular to the inclined edge in the
    front view)

Step 3: Project points from the front view to the auxiliary plane

    Projection lines are drawn perpendicular to the
    auxiliary plane (parallel to the projection direction)

Step 4: Construct the auxiliary view using projected points

    AUXILIARY VIEW (true shape):
    ┌─────────────────────────┐
    │                         │
    │    ┌───────────┐        │
    │    │  RECT.    │        │  ← Shows TRUE dimensions
    │    │  POCKET    │        │     40mm × 25mm
    │    │           │        │
    │    └───────────┘        │
    │                         │
    └─────────────────────────┘

Step 5: Verify the result
        - Rectangle dimensions are now TRUE SIZE
        - Parallel lines remain parallel
        - Angles on the inclined plane are preserved
```

### 2.3.3 Example 2.5: Finding True Length on an Inclined Edge

**Problem:** Determine the true length of edge AB, which is inclined at 45° to the horizontal plane.

**Solution:**

```
Step 1: Draw the front view and top view of edge AB

    FRONT VIEW:          TOP VIEW:
    A'                    A"
    ●────────────────●   ●────────────────●
    B'                   B"
    
    A'B' shows vertical height change
    A"B" shows horizontal run

Step 2: Construct a true-length diagram

    Use the front view and top view to calculate:
    True Length² = (Horizontal Run)² + (Vertical Rise)²
    
    Example: If top view shows 60mm run and front view
            shows 60mm rise, then:
            
    True Length = √(60² + 60²) = √7200 = 84.85mm

Step 3: Verify using auxiliary projection

    Draw auxiliary view where the edge projects in true length
    by making the auxiliary plane parallel to the edge AB
```

## 2.4 Projection Practice Problems

### Problem Set 2.1: Basic Projection

**Problem 2.1.1:** Draw the front, top, and right-side views of a hexagonal prism (25mm across flats, 40mm height) with a 10mm diameter through hole centered on the axis.

**Problem 2.1.2:** Draw a rectangular plate (80mm × 60mm × 10mm thick) with four 8mm diameter holes in each corner, positioned 10mm from each edge.

**Problem 2.1.3:** Draw a cylindrical shaft (30mm diameter, 100mm long) with a keyway on one end. Keyway is 6mm wide × 4mm deep × 20mm long.

### Problem Set 2.2: View Selection

**Problem 2.2.1:** A taper is turned on a shaft such that one end is 20mm diameter and the other is 30mm diameter over a length of 50mm. Select and draw appropriate views.

**Problem 2.2.2:** A sheet metal bracket has been bent at 90° with dimensions 100mm × 60mm in the plane of each leg, and 2mm thick. Select views.

**Problem 2.2.3:** A welded assembly consists of two tubes (40mm OD, 30mm ID) welded perpendicular to each other. Select views.

## 2.5 Common Mistakes in Orthographic Projection

### Mistake 1: Misaligned Features

**Symptom:** Holes, slots, or edges that should align between views are visibly offset.

**Cause:** Failing to project construction lines between views before drawing final features.

**Correction:**
```
WRONG:                           CORRECT:
┌──────┐                         ┌──────┐
│  ○   │──┐                      │      │
│      │  │                      │  ○   │
└──────┘  │                      │      │
         │                      └──────┘
         │                           │
         ▼                           ▼
    Top View: hole not centered  Top View: hole correctly centered
```

### Mistake 2: Projecting in Wrong Direction

**Symptom:** Views appear as mirror images of the object.

**Cause:** Projecting from the wrong side or confusing first/third angle rules.

**Correction:** Verify projection system before starting. Double-check which side of the fold line each view belongs to.

### Mistake 3: Extraneous Views

**Symptom:** Drawing includes unnecessary views that clutter the sheet.

**Cause:** Over-caution or misunderstanding of minimum view requirements.

**Correction:** Ask: "What would I not know without this view?" If the answer is nothing, the view may be unnecessary.

## 2.6 References and Further Reading

- **ISO 128-2:2020** — Presentation of views and sections
- **Madsen, D.A., et al.** — *Engineering Drawing and Design*, Delmar Cengage Learning
- **French Standard NF E04-012** — Technical drawings — Methods of projection (first angle)
- **American National Standard ASME Y14.3-2019** — Multi-view and section view drawings

---

# 3. Line Types and Their Applications

## 3.1 Introduction to Line Conventions

Line conventions in technical drawing are not arbitrary stylistic choices but standardized systems that convey specific types of information. Each line type has a defined meaning, and the consistent application of these conventions ensures that all readers interpret drawings identically.

### 3.1.1 The Five Fundamental Line Types

The international standard ISO 128-20 defines five fundamental line types, each with specific applications:

| Line Type | Visual Appearance | Standard Width | Primary Applications |
|-----------|------------------|----------------|---------------------|
| Thick continuous | ━━━━━━━━━━━━━━ | 0.5–0.7 mm (varies with drawing size) | Visible edges, outlines |
| Thin continuous | ─────────────── | 0.25–0.35 mm | Imaginary edges, hatching, dimensions |
| Thick dashed | ━ ━ ━ ━ ━ ━ ━ ━ | 0.5–0.7 mm | Cutting plane lines |
| Thin dashed | - - - - - - - - - | 0.25–0.35 mm | Hidden edges, hidden threads |
| Thin chain | ━ ━ ━ ━ ━ ━ ━ ━ ━ | 0.25–0.35 mm | Centerlines, symmetry planes |
| Thin chain (double dash) | ━ ━ ━ ━ ━ ━ ━ ━ ━ | 0.25–0.35 mm | Outlines of nearby parts, extreme positions |

### 3.1.2 Line Width Standards

**General Principles:**

1. **Two widths only:** Every line on a technical drawing should be either thick or thin (there is no medium line weight in standard practice)

2. **Consistent ratio:** The ratio between thick and thin lines is typically 2:1 or 3:2

3. **Minimum practical widths:** For small drawings, use minimum 0.25mm (thin) and 0.5mm (thick)

4. **Large format scaling:** For very large drawings, line widths may increase proportionally

**Line Width Selection Table:**

| Drawing Sheet Size | Thin Line Width | Thick Line Width |
|-------------------|-----------------|------------------|
| A4, A3 | 0.25 mm | 0.5 mm |
| A2, A1 | 0.35 mm | 0.7 mm |
| A0 | 0.5 mm | 1.0 mm |

## 3.2 Thick Continuous Lines

### 3.2.1 Definition and Appearance

The **thick continuous line** (also called **visible outline** or **object line**) is drawn with the drawing's maximum line width. It represents features that are visible from the observer's viewpoint and form the outer boundaries or prominent edges of the object.

**Technical Specification:**
```
Line Type Code: ISO 01.1 (thick continuous)
Line Width: w (the designated thick width, e.g., 0.5 mm)
Dash Pattern: Solid (no breaks)
Examples in ASCII:
━━━━━━━━━━━━━━━  (visible outline)
━━━━━━━━━━━━━━━  (outer contour)
```

### 3.2.2 Primary Applications

**Application 1: Visible Edges and Outlines**

Every edge of the object that is visible from the viewing direction is drawn as a thick continuous line. This includes:

- Outer contours of the object
- Edges between surfaces meeting at an angle
- Edges where a curved surface meets a plane
- Boundaries between different visible features

**Example 3.1: Identifying Visible Edges**

```
Drawing of a stepped shaft:

    FRONT VIEW:              TOP VIEW:
    ┌────────────────────┐   ┌──────────────────┐
    │                    │   │ ●               │ ← Thick: outer
    │    ████████████    │   │   ●────────●     │    contour
    │    ████████████    │   │   ●────────●     │    (circles)
    │════════════════════│   │   ●────────●     │ ← Thick: step
    │    ████████████    │   │   ●────────●     │    visible
    │    ████████████    │   │   ●────────●     │
    │                    │   │                  │
    └────────────────────┘   └──────────────────┘
    
    Thick lines show:
    - The outer boundary of each diameter
    - The step between diameters
    - The ends of the shaft
```

**Application 2: Outlines of Removed Sections**

When a section view is taken, the cutting plane line is thick dashed, but the outline of the remaining portion of the object (outside the section) remains thick continuous.

**Application 3: Arrows Showing Viewing Direction**

The arrows at the ends of cutting plane lines are drawn with thick lines to ensure visibility.

### 3.2.3 Common Errors with Thick Lines

| Error | Consequence | Prevention |
|-------|-------------|------------|
| Line too thin | Drawing appears weak; features may be missed | Maintain consistent pencil pressure or use mechanical pencil with correct lead |
| Line varies in width | Drawing appears unprofessional; confusion about edge location | Keep pencil sharp; do not press harder to compensate for dullness |
| Using thick line for hidden features | Hidden features appear visible | Always use thin dashed lines for hidden edges |

## 3.3 Thin Continuous Lines

### 3.3.1 Definition and Appearance

The **thin continuous line** is drawn with the drawing's minimum line width. It represents imaginary or theoretical features, construction geometry, and supplementary information.

**Technical Specification:**
```
Line Type Code: ISO 01.2 (thin continuous)
Line Width: w/2 or w/3 (e.g., 0.25 mm)
Dash Pattern: Solid (no breaks)
Examples in ASCII:
───────────────  (construction)
───────────────  (hatching)
```

### 3.3.2 Primary Applications

**Application 1: Imaginary Edges**

Imaginary edges are theoretical intersections that would occur if fillet radii were extended to sharp edges, or if curved surfaces were flattened.

**Example 3.2: Drawing Fictitious Edges on a Cast Part**

```
A cast housing with large fillets:

    BEFORE (with fillets):       AFTER (fictitious edges shown):
    ┌──────────────────┐          ┌──────────────────┐
    │                  │          │   \            /  │
    │   (curved)       │          │    \──────────/   │ ← Thin continuous
    │                  │          │   /   (curved) \  │    fictitious edge
    └──────────────────┘          └──/              \─┘
    
    The fictitious edge shows where the surface 
    would intersect if the fillet were not present.
```

**Application 2: Hatching (Section Fill)**

Hatching lines drawn with thin continuous strokes fill sectioned areas to indicate the material type.

**Application 3: Dimension and Extension Lines**

Dimension lines and their associated extension lines are thin continuous.

**Application 4: Outlines of Revolved Sections**

When a revolved section is drawn directly on a view, its outline uses thin continuous lines.

**Application 5: Visible Thread Roots**

The crests (outer edges) of external threads and the roots (inner edges) of internal threads are shown as thin continuous lines when the thread is shown in simplified representation.

**Application 6: Limits of Local Sections**

Local sections are bounded by thin freehand wavy lines, which are thin continuous.

### 3.3.3 Example 3.3: Thin Continuous Line Applications

```
COMPLETE DRAWING SHOWING MULTIPLE THIN LINE USES:

    ┌────────────────────────────────────────────────┐
    │          ╲  SECTION A-A                       │
    │           ╲                                  │
    │            ━━━━━━━━━━━━━━━━━━━━━━  ← Thick:  │ ← Thick: cutting
    │            (arrows at ends)           cutting │    plane line
    │             plane line                    line │
    ├────────────────────────────────────────────────┤
    │                                                │
    │  ┌───────────────────────────────┐            │
    │  │░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│ ← Thin:    │ ← Thin:
    │  │░░░░ HATCHING (section)   ░░░░░│   hatching │    hatching
    │  │░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│            │
    │  └───────────────────────────────┘            │
    │          ↑                                     │
    │    Thin continuous hatching                    │
    │                                                │
    │  ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─  ← Thin:     │
    │  0        50       100       150        center │
    │  ├────────┼────────┼────────┼─────→   line   │
    │          │        │        │                │
    │  Dimension value (placed on line or above)   │
    │                                                │
    └────────────────────────────────────────────────┘
    
    LEGEND:
    ────────  Thick continuous: visible outlines
    ─ ─ ─ ─   Thin continuous: hatching, dimensions, centerlines
```

## 3.4 Thin Dashed Lines

### 3.4.1 Definition and Appearance

The **thin dashed line** (ISO 02.1) represents features that are not directly visible from the observer's viewpoint because they are behind other surfaces or inside cavities.

**Technical Specification:**
```
Line Type Code: ISO 02.1 (thin dashed)
Line Width: w/2 or w/3 (e.g., 0.25 mm)
Dash Pattern: 3mm long dashes with 1mm gaps
Visual Appearance: - - - - - - - - - - -
```

### 3.4.2 Primary Applications

**Application 1: Hidden Edges and Contours**

Any edge or surface that is obscured by material in front of it is shown as a thin dashed line.

**Example 3.4: Hidden Hole in a Block**

```
FRONT VIEW (external):        TOP VIEW:
┌──────────────────┐          ┌──────────────────┐
│                  │          │                  │
│                  │          │                  │
│                  │          │                  │
│                  │          │                  │
└──────────────────┘          └──────────────────┘

FRONT VIEW (with hidden        TOP VIEW (shows
feature implied):              true circular hole):
┌──────────────────┐          ┌──────────────────┐
│                  │          │        ○         │
│                  │          │       ( )        │ ← Thin dashed:
│                  │          │        ○         │    hidden hole
│                  │          │                  │
└──────────────────┘          └──────────────────┘

The front view does NOT show the hole because the
front face is continuous. The top view shows the
hole with thin dashed lines because it is on the
upper surface.
```

**Application 2: Hidden Threads**

Internal threads that cannot be seen from the current view direction are represented with thin dashed lines.

**Application 3: Hidden Tapped Holes**

In a section view, the threaded portion of a tapped hole below the entrance may be shown with thin dashed lines.

### 3.4.3 Dashed Line Best Practices

**Rule 1: Do not start or end with a gap**

In most standards, dashed lines should begin with a full dash, not a gap. However, when a dashed line meets a visible line at an edge, the dashed line should end with a dash (not a gap).

**Rule 2: Corner treatment**

```
CORRECT:                       INCORRECT:
    ┌───────────────┐               ┌───────────────┐
    │ - - - - - - - │               │   - - - - -  │
    │               │               │               │
    │           - - │ - - - - - -   │           - -│- - - - -
    └───────────────┘               └───────────────┘
    
    Dashed line ends meet visible     Gaps at corners
    line at a dash                    create confusion
```

**Rule 3: Spacing consistency**

Maintain uniform dash length and gap spacing throughout the drawing. The standard ratio is typically 3:1 (3mm dash, 1mm gap for thin dashed lines at 1:1 scale).

**Example 3.5: Multiple Hidden Features**

```
DRAWING OF A STEPPED CYLINDER WITH INTERNAL FEATURES:

    SECTION A-A (full section):
    ┌────────────────────────────┐
    │                            │
    │  ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─   │ ← Thin dashed: 
    │  │                   │ │   │    hidden thread
    │  │   INNER BORE      │ │   │
    │  │  (hidden surface)  │ │   │
    │  │                   │ │   │
    │  ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─   │
    │                            │
    │   ████████████████████     │ ← Thick: outer
    │   ████████████████████     │    contour
    │                            │
    └────────────────────────────┘
```

## 3.5 Thin Chain Lines

### 3.5.1 Definition and Appearance

The **thin chain line** (also called **centerline** or **dash-dot line**) has long and short dashes alternating regularly. It indicates axes of symmetry, centerlines of cylindrical features, and reference planes.

**Technical Specification:**
```
Line Type Code: ISO 04.1 (thin chain line)
Line Width: w/2 or w/3 (e.g., 0.25 mm)
Dash Pattern: 12mm long dashes with 2mm gaps, alternating with 
              2mm short dashes
Visual Appearance: ━ ━ ━ ━ ━ ━ ━ ━ ━
```

### 3.5.2 Primary Applications

**Application 1: Axes of Rotation and Symmetry**

Centerlines indicate the axis about which a rotational feature (cylinder, cone, etc.) is generated. They also indicate planes of symmetry.

**Example 3.6: Centerlines on a Shaft**

```
FRONT VIEW:                    TOP VIEW:
        │                              ─ ─ ─ ─
        │   ┌──────────────┐          ─ ─ ─ ─
        │   │              │          ╱       ╲
        │   │              │         ╱         ╲
        │   │              │        │           │
        │   │              │        │     ●     │ ← Center point
        │   │              │        │           │
        │   │              │         ╲         ╱
        │   │              │          ╲       ╱
        │   │              │          ─ ─ ─ ─
        │   └──────────────┘          ─ ─ ─ ─
        │                                   
    ┌───┴───┐ ← Long dash-dash-dash dash pattern
    │       │
    
    The centerline:
    - Passes through the exact center of cylindrical features
    - Extends slightly beyond the feature boundaries
    - Has small gaps where it intersects visible outlines
```

**Application 2: Gear Pitch Circles**

On gear drawings, the pitch circle (theoretical circle where teeth mesh) is indicated with a thin chain line.

**Application 3: Bolt Circle Centerlines**

Multiple holes arranged in a circular pattern have a centerline through the center of the pattern, with a pitch circle at the bolt circle diameter.

**Example 3.7: Centerlines on a Flange with Holes**

```
TOP VIEW OF FLANGE WITH 6 HOLES:

              - - - - - - - - -
            -                   -
           -                     -
          -                       -
         -          ●              -      ← Center point
          -                       -        (small cross)
           -                     -
            -                   -
              - - - - - - - - -
                     │
                     │ Pitch circle (bolt circle)
                     │ thin chain line
                     
    Each hole center is marked with a small cross
    intersecting the pitch circle
```

### 3.5.3 Chain Line Termination Rules

**Standard Termination:**
1. Chain lines should extend 2-5mm beyond the outermost features they reference
2. Chain lines should not terminate in gaps when they meet visible outlines
3. At intersections, short dashes cross at the intersection point

**Special Cases:**
- Chain lines for cylindrical features pass through the circular ends
- Chain lines may have small gaps at intersections with visible lines
- Symmetry plane lines extend to show the full extent of the symmetry

## 3.6 Thin Chain Lines with Two Dashes

### 3.6.1 Definition and Appearance

The **thin chain line with two dashes** (ISO 04.2) is a variant of the standard chain line with short dashes at both ends. It is used for specific applications where additional emphasis is needed.

**Technical Specification:**
```
Line Type Code: ISO 04.2 (thin chain line with two dashes)
Line Width: w/2 or w/3 (e.g., 0.25 mm)
Dash Pattern: Short dash at each end, long dashes with short 
              dash alternations in middle
Visual Appearance: ━- ━ ━- ━ ━- ━ ━
```

### 3.6.2 Primary Applications

**Application 1: Outlines of Nearby Parts**

When showing an adjacent part that is not in direct contact, its outline is drawn with thin chain line with two dashes.

**Example 3.8: Adjacent Part Representation**

```
DRAWING SHOWING BEARING ON SHAFT:

    ┌──────────────────────────────────────────┐
    │                                          │
    │     ╔══════════════════╗                  │
    │     ║                  ║  ← Thick: Shaft │
    │     ║     BEARING      ║                  │
    │     ║                  ║  ← Thin chain   │
    │     ╚══════════════════╝     with two     │
    │              ╱╲            dashes:       │
    │             ╱  ╲           Adjacent part │
    │            ╱    ╲                        │
    │           ╱      ╲                       │
    └──────────────────────────────────────────┘
```

**Application 2: Extreme Positions of Moving Parts**

When a part has a range of motion, one position is shown with thick lines (the stationary or primary position), and alternative positions are shown with thin chain line with two dashes.

**Example 3.9: Piston Extreme Positions**

```
DRAWING SHOWING PISTON TRAVEL RANGE:

    ┌──────────────────────────────────────────┐
    │                                          │
    │  ─ ─ ┬─────────────────────────────      │ ← Upper limit
    │  ─ ─ │                                     │   (chain with
    │      │    ╔══════════════╗                │    two dashes)
    │      │    ║              ║                │
    │      │    ║    PISTON    ║ ← Thick:       │
    │      │    ║   (current)  ║   current       │
    │      │    ║              ║   position     │
    │      │    ╚══════════════╝                │
    │      │                                     │
    │  ─ ─ ┴─────────────────────────────       │ ← Lower limit
    │  ─ ─                                     │   (chain with
    │                                          │    two dashes)
    └──────────────────────────────────────────┘
```

**Application 3: Revolved Half-View Boundaries**

When a revolved half-section is attached to a main view, the boundary between the revolved portion and the exterior view is shown with thin chain line with two dashes.

## 3.7 Line Type Selection Guide

### 3.7.1 Decision Matrix for Line Selection

| Situation | Required Line Type | Standard Code |
|----------|-------------------|---------------|
| Outer boundary of object | Thick continuous | ISO 01.1 |
| Visible edge of feature | Thick continuous | ISO 01.1 |
| Edge at tangent to surface | Thick continuous | ISO 01.1 |
| Imaginary intersection (fillet) | Thin continuous | ISO 01.2 |
| Section hatching | Thin continuous | ISO 01.2 |
| Dimension lines | Thin continuous | ISO 01.2 |
| Extension lines | Thin continuous | ISO 01.2 |
| Hidden edge (inside cavity) | Thin dashed | ISO 02.1 |
| Hidden thread root | Thin dashed | ISO 02.1 |
| Centerline/axis of rotation | Thin chain | ISO 04.1 |
| Plane of symmetry | Thin chain | ISO 04.1 |
| Bolt circle | Thin chain | ISO 04.1 |
| Outline of nearby part | Chain with two dashes | ISO 04.2 |
| Extreme position of moving part | Chain with two dashes | ISO 04.2 |
| Cutting plane line | Thick dashed | ISO 02.2 |

### 3.7.2 Example 3.10: Complete Line Type Analysis

```
PROBLEM: Identify the line types in the drawing below

TOP VIEW:
      - - - - - - - - - - -
    -                     -
   -                       -
  -                         -
 -           ●               -    ← Thin chain: bolt circle
  -                         -      Center point: thin cross
   -                       -
    -                     -
      - - - - - - - - - - -

FRONT VIEW:
┌─────────────────────────────┐
│                             │
│    ╔═══════════════════╗    │ ← Thick: visible outline
│    ║   ┌─────────────┐ ║    │
│    ║   │ ░░░░░░░░░░░░ │ ║    │ ← Thin: hatching
│    ║   │ ░░░░░░░░░░░░ │ ║    │
│    ║   │ ░░░░░░░░░░░░ │ ║    │
│    ║   └─────────────┘ ║    │
│    ╚═══════════════════╝    │
│            │                │ ← Thin chain: centerline
│            │                │ ← Thin dashed: hidden hole
│           - -               │    edge
└─────────────────────────────┘
```

## 3.8 Common Mistakes with Line Types

### Mistake 1: Using Visible Lines for Hidden Features

**Symptom:** Features that should be hidden appear as solid outlines.

**Problem:** This could mislead the reader into thinking the feature is on the surface rather than inside or behind.

**Correction:** Always use thin dashed lines (ISO 02.1) for hidden edges.

### Mistake 2: Inconsistent Line Weights

**Symptom:** Visible outlines appear to vary in thickness throughout the drawing.

**Problem:** Creates visual confusion; may suggest the drawing is incomplete or unprofessional.

**Correction:** Use a consistent pencil or drawing instrument. Check line weights against a standard sheet periodically.

### Mistake 3: Mixing First and Third Angle Rules

**Symptom:** Views appear inconsistent with each other.

**Problem:** Fundamental projection error.

**Correction:** Always verify which projection system you are using and apply its rules consistently.

### Mistake 4: Overusing Centerlines

**Symptom:** Centerlines drawn through every cylindrical feature, creating visual clutter.

**Problem:** Excessive centerlines reduce readability.

**Correction:** Draw centerlines only where they serve a purpose: showing symmetry, indicating bolt circles, or marking reference axes.

### Mistake 5: Incorrect Hatching Direction

**Symptom:** Hatching lines intersect with visible outlines or dimension lines inappropriately.

**Problem:** Violates standard hatching rules.

**Correction:** Ensure hatching stops 1-2mm short of visible outlines and does not cross thick lines.

## 3.9 Line Work Exercises

### Exercise Set 3.1: Identifying Line Types

**Exercise 3.1.1:** Given a complex assembly drawing, identify each line type and explain its significance.

**Exercise 3.1.2:** Redraw the following representation, correctly applying line types:

```
WRONG DRAWING: (all lines same type)

┌──────────────────────┐
│   ○     - - - -       │
│       ○  - - - -      │
│           - - - -    │
└──────────────────────┘

CORRECTED: (identify and fix line types)
```

### Exercise Set 3.2: Applying Line Types

**Exercise 3.2.1:** Draw a cylindrical housing showing:
- External visible outline (thick)
- Internal hidden bore (thin dashed)
- Centerline of bore (thin chain)
- Section hatching (thin continuous)
- Adjacent mounting flange outline (chain with two dashes)

**Exercise 3.2.2:** Draw a bolted joint assembly showing:
- Bolt head (thick outline)
- Tapped hole in plate (thin dashed)
- Bolt centerline (thin chain)
- Adjacent washer outline (chain with two dashes)
- Section through bolted joint

## 3.10 References and Further Reading

- **ISO 128-20:1999** — Lines
- **ISO 128-24:1999** — Lines on mechanical engineering drawings
- **ASME Y14.2M-2019** — Lines, Lettering, and Writing
- **Bhatt, N.D.** — *Engineering Drawing*, Charotar Publishing House

---

# 4. Drawing Formats and Documentation Standards

## 4.1 The A-Series Drawing Formats

The international standard for paper sizes, known as the A-series, was first established in Germany in 1922 (DIN 476) and subsequently adopted internationally. This system provides a rational, mathematically consistent approach to sheet sizing.

### 4.1.1 Understanding the A-Series System

**Fundamental Principle:** All A-series sheets have the same aspect ratio: √2:1 (approximately 1:1.414). This special ratio means that when a sheet is halved parallel to its shorter side, the resulting sheet maintains the same aspect ratio.

**Mathematical Derivation:**

```
If width = a and height = b, with b/a = √2

Then when folded in half:
New width = b/2
New height = a

New ratio = (b/2)/a = b/(2a) = (√2 × a)/(2a) = √2/2 = 1/√2

But this is not √2:1...

The actual DIN system uses a different arrangement:
- A0 has area of exactly 1 square meter
- Width = 841mm (approximately 1/√2 meters)
- Height = 1189mm (approximately 1 meter)
- Ratio = 841/1189 ≈ 0.707 ≈ 1/√2

When A0 is halved:
- Each A1 sheet: 594mm × 841mm
- Half of 1189mm is 594.5mm (rounded to 594mm)
- Ratio = 594/841 ≈ 0.706 ≈ 1/√2 ✓
```

### 4.1.2 Standard A-Series Dimensions

| Format | Dimensions (mm) | Dimensions (inches) | Area (m²) | Relative Size |
|--------|-----------------|---------------------|-----------|---------------|
| A0 | 841 × 1189 | 33.1 × 46.8 | 1.000 | 1 |
| A1 | 594 × 841 | 23.4 × 33.1 | 0.500 | 1/2 of A0 |
| A2 | 420 × 594 | 16.5 × 23.4 | 0.250 | 1/4 of A0 |
| A3 | 297 × 420 | 11.7 × 16.5 | 0.125 | 1/8 of A0 |
| A4 | 210 × 297 | 8.27 × 11.69 | 0.0625 | 1/16 of A0 |
| A5 | 148 × 210 | 5.83 × 8.27 | 0.0313 | 1/32 of A0 |
| A6 | 105 × 148 | 4.13 × 5.83 | 0.0156 | 1/64 of A0 |

**Example 4.1: Selecting Appropriate Format**

**Scenario:** You need to draw a precision mechanical part measuring approximately 150mm × 80mm × 40mm with multiple views and detailed dimensions.

**Analysis:**
```
Part dimensions: 150mm × 80mm × 40mm

Minimum drawing area required:
- 3 views (front, top, side): approximately 200mm × 150mm
- Dimension and note areas: approximately 50mm margins
- Title block area: 40mm minimum
- Total minimum: approximately 300mm × 250mm

Recommended format: A3 (297mm × 420mm)
- Provides adequate margins
- Allows enlargement of small features as details
- Manageable size for filing and handling
- Standard for most engineering drawings

Alternative: A4 could work but would require:
- Reduced scale (1:1 or 1:2)
- Multiple detail views
- Compressed dimension placement
- Generally not recommended for complex parts
```

### 4.1.3 Margins and Drawing Area

**ISO 5457 Standard Margins:**

| Format | Left Margin (mm) | Other Margins (mm) |
|--------|------------------|--------------------|
| A0, A1 | 20 | 10 |
| A2, A3, A4 | 20 | 10 |

The larger left margin serves several purposes:
1. **Filing:** Allows holes for binding without damaging drawing content
2. **Handling:** Provides a margin for holding the sheet
3. **Protection:** Shields drawing content from wear

**Example 4.2: Margin Application**

```
A3 SHEET LAYOUT:

    ┌─────────────────────────────────────────────────┐
    │                                                 │
    │ 20mm  │← ← ← DRAWING AREA → → →│  10mm          │
    │ MARGIN│                            │ MARGIN     │
    │       │                            │            │
    │       │    ┌──────────────────┐    │            │
    │       │    │                  │    │            │
    │       │    │   TITLE BLOCK   │    │            │
    │       │    │   (bottom right) │    │            │
    │       │    │                  │    │            │
    │       │    └──────────────────┘    │            │
    │       │                            │            │
    │       │                            │            │
    └───────┴────────────────────────────┴────────────┘
           │                                            │
           │              420mm TOTAL WIDTH             │
           └────────────────────────────────────────────┘
                              │
                    297mm TOTAL HEIGHT
```

## 4.2 Title Blocks

The title block is a critical component of any technical drawing. It serves as the drawing's "identity card," containing all the information necessary to identify, classify, interpret, and use the drawing correctly.

### 4.2.1 Purpose and Importance of Title Blocks

**Primary Functions:**

1. **Identification:** Provides unique drawing number, revision, and sheet information
2. **Administrative:** Contains dates, names, and organizational information
3. **Technical:** Specifies scale, units, projection method, and material
4. **Contractual:** Establishes the document's legal status and approval

### 4.2.2 Standard Title Block Layout

**ISO 7200 Standard Format:**

```
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│  COMPANY LOGO                                      DRAWING NUMBER   │
│  AND/OR                                             ─────────────   │
│  NAME                                               Sheet __ of __  │
│                                                     (if multipage)  │
│─────────────────────────────────────────────────────────────────────│
│                                                                     │
│                                                                     │
│  TITLE OF DRAWING                                                   │
│  ─────────────────────────────────────────────────────────          │
│                                                                     │
│─────────────────────────────────────────────────────────────────────│
│                                                                     │
│  SCALE   │  DATE    │  DRAWN │  CHECKED │  APPROVED │  REV        │
│  ────────│──────────│────────│──────────│───────────│────────    │
│  1:2     │ 2024-01  │  J.Smith│ M.Brown │  T.Wilson  │ A          │
│          │          │        │          │            │            │
│─────────────────────────────────────────────────────────────────────│
│                                                                     │
│  MATERIAL                                    WEIGHT                │
│  ─────────────────────────────────────────── ──────                │
│  Steel, S355JR                              2.35 kg                │
│                                             (if applicable)        │
│─────────────────────────────────────────────────────────────────────│
│                                                                     │
│  TOLERANCE STANDARD                        PROJECTION SYMBOL       │
│  ──────────────────────────────────────── ────────────────────      │
│  ISO 2768-m                                 [First angle symbol]    │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### 4.2.3 Title Block Fields Explained

**Drawing Number:**
- Unique identifier assigned by the organization
- Often follows a coding system (e.g., DEPT-PROJECT-SEQUENCE)
- Example: "MECH-2024-00145"

**Title:**
- Clear, concise description of what is shown
- Should allow someone to distinguish from similar drawings
- Example: "PUMP HOUSING, MODEL A-15"

**Scale:**
- Ratio of drawing size to actual size
- Written as "1:1" (full size), "1:2" (half size), "2:1" (enlarged)
- Never use verbal forms like "HALF SIZE"

**Date:**
- Typically the date of original issue or latest revision
- ISO format: YYYY-MM or YYYY-MM-DD

**Personnel Fields:**
- Drawn: Name or initials of the person who created the drawing
- Checked: Name or initials of the person who verified accuracy
- Approved: Name or initials of person with approval authority

**Revision:**
- Letter or number indicating the revision level
- Revision history may be shown in a separate table

**Material:**
- Material designation per applicable standard
- Important for manufacturing and procurement

**Projection Symbol:**
- Indicates first-angle or third-angle projection
- Required by ISO 128

**Tolerance Standard:**
- Reference to general tolerance standard applied
- Example: ISO 2768-m (general tolerances for linear dimensions)

### 4.2.4 Example 4.3: Complete Title Block for an Assembly Drawing

```
┌──────────────────────────────────────────────────────────────────────────┐
│                                                                          
│  ACME MECHANICAL INC.                                 DWG NO: AMI-4472-B  │
│  ┌────────────┐                                       SHEET 1 OF 3      │
│  │    ACME     │                                                         │
│  │   (logo)    │                                                         │
│  └────────────┘                                                         │
│──────────────────────────────────────────────────────────────────────────│
│                                                                          
│                        HYDRAULIC CYLINDER ASSEMBLY                        │
│                        ─────────────────────────                          │
│                        MODEL HC-200, DOUBLE ACTING                        │
│                                                                          
│──────────────────────────────────────────────────────────────────────────│
│                                                                          
│  SCALE    │   DATE    │  DRAWN  │  CHKD   │  APPRVD  │  REV              │
│  ──────── │ ───────── │ ─────── │ ─────── │ ──────── │ ────             │
│  1:4      │ 2024-03   │  R.Lee  │  K.Park │  J.Wong  │ B               │
│                                                                          
│──────────────────────────────────────────────────────────────────────────│
│                                                                          
│  MATERIAL                                            NET WEIGHT          │
│  ──────────────────────────────────────────────────  ──────────          │
│  SEE BOM (SHEET 3)                                   12.7 kg           │
│                                                                          
│──────────────────────────────────────────────────────────────────────────│
│                                                                          
│  GENERAL TOLERANCES                             PROJECTION               │
│  ──────────────────────────────────────────────  ─────────────          │
│  ISO 2768-m                                       [FIRST ANGLE]         │
│                                                                          
└──────────────────────────────────────────────────────────────────────────┘
```

## 4.3 Drawing Scales

Scale is the ratio between the size of the drawing and the actual size of the object it represents. Proper scale selection is essential for clarity, accuracy, and practical drawing creation.

### 4.3.1 Scale Notation

**ISO Standard Scale Designation:**

| Scale Type | Designation | Application |
|------------|-------------|-------------|
| Enlargement | 50:1, 20:1, 10:1, 5:1, 4:1, 2:1 | Very small objects or features |
| Full size | 1:1 | Objects of moderate size |
| Reduction | 1:2, 1:5, 1:10, 1:20, 1:50, 1:100, 1:200, 1:500, 1:1000 | Large objects |
| Metric preference | Powers of 1, 2, 5, 10 | Standard practice |

### 4.3.2 Scale Selection Guidelines

**Factors to Consider:**

1. **Object Size:** Larger objects require smaller scales
2. **Feature Size:** Small features need larger scales to show clearly
3. **Drawing Sheet Size:** Fit the drawing within available space
4. **Dimension Readability:** Ensure dimension text remains legible
5. **Reproduction:** Consider reduction for printing/archiving

**Scale Selection Table:**

| Object Characteristic Dimension | Recommended Scale Range |
|--------------------------------|------------------------|
| < 10 mm | 2:1, 5:1, 10:1 (enlargement) |
| 10 - 50 mm | 1:1, 2:1 |
| 50 - 200 mm | 1:1, 1:2, 1:5 |
| 200 - 1000 mm | 1:5, 1:10, 1:20 |
| 1 - 5 m | 1:20, 1:50, 1:100 |
| 5 - 50 m | 1:50, 1:100, 1:200 |
| > 50 m | 1:200, 1:500, 1:1000 |

**Example 4.4: Scale Selection for a Precision Instrument Part**

```
Part: Precision optical mount bracket
Material: Aluminum 6061-T6
Overall dimensions: 85mm × 60mm × 25mm
Critical features:
- Central bore: 30mm diameter, ±0.02mm tolerance
- Mounting holes: 4 × M3 threaded, ±0.05mm position tolerance
- Surface preparation: 0.8 μm Ra on mating surfaces

SCALE ANALYSIS:

Option A: 1:1 (full size)
- Pros: Direct measurement, easy visualization
- Cons: May not fit all features clearly on A4
- Verdict: RECOMMENDED - parts fit well on A4/A3

Option B: 1:2 (half size)
- Pros: Fits easily on A4
- Cons: Dimension text may be small, loses detail clarity
- Verdict: Acceptable for overall view only

Option C: 2:1 (double size)
- Pros: Shows critical features clearly
- Cons: Would require multiple sheets
- Verdict: Good for detail views of bore

FINAL RECOMMENDATION:
- Main views: 1:1
- Detail of bore: 2:1 or full size
```

### 4.3.3 Scale Placement on Drawings

**Standard Practice:**

1. Scale is specified in the title block for the entire drawing
2. Detail views that differ from the main scale must indicate their own scale
3. The notation follows the format: "SCALE 1:2" or simply "1:2"
4. When multiple scales are used, a **scale block** may be added near the drawing area

**Example 4.5: Multiple Scale Notation**

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                          MAIN VIEW                              │
│                        SCALE 1:2                                │
│                    ┌───────────────────┐                       │
│                    │                   │                       │
│                    │    ASSEMBLY       │                       │
│                    │                   │                       │
│                    └───────────────────┘                      │
│                                                                 │
│                           ┌─────────────┐                       │
│                           │  DETAIL A   │ ← Enlarged feature   │
│                           │  (Note: 2:1)│    Scale shown       │
│                           │   ┌─────┐   │                       │
│                           │   │  ○  │   │                       │
│                           │   └─────┘   │                       │
│                           └─────────────┘                       │
│                                                                 │
│   ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─   │
│   0     10    20    30    40    50    60    70    80    90     │
│   ├─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────   │
│                         DIMENSION LINE (on drawing)             │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

## 4.4 Drawing Frame and Border

### 4.4.1 Purpose of Drawing Frames

The drawing frame (border) serves both practical and aesthetic purposes:

1. **Defines Drawing Area:** Establishes clear boundaries for content
2. **Provides Margins:** Creates a clean edge for handling and filing
3. **Professional Appearance:** Gives the drawing a polished look
4. **Zone Marking:** Enables location referencing for communication

### 4.4.2 Zone Marking System

**ISO 5457 Zone System:**

The drawing area is divided into zones by imaginary grid lines, typically 50mm apart for A0-A2 and 25mm apart for A3-A4. Zones are referenced by letters (vertical) and numbers (horizontal).

```
ZONE MARKING ON A3 SHEET:

    ┌─────┬─────┬─────┬─────┬─────┬─────┐
    │     │     │     │     │     │     │
    │  A  │  B  │  C  │  D  │  E  │  F  │   ← Horizontal
    │     │     │     │     │     │     │     zones
────┼─────┼─────┼─────┼─────┼─────┼─────┼────
    │     │     │     │     │     │     │
    │ 1   │ 1   │ 1   │ 1   │ 1   │ 1   │
    │     │     │     │     │     │     │
────┼─────┼─────┼─────┼─────┼─────┼─────┼────
    │     │     │     │     │     │     │
    │ 2   │ 2   │ 2   │ 2   │ 2   │ 2   │
    │     │     │     │     │     │     │
────┼─────┼─────┼─────┼─────┼─────┼─────┼────
    │     │     │     │     │     │     │
    │ 3   │ 3   │ 3   │ 3   │ 3   │ 3   │
    │     │     │     │     │     │     │
────┼─────┼─────┼─────┼─────┼─────┼─────┼────
    │     │     │     │     │     │     │
    │ 4   │ 4   │ 4   │ 4   │ 4   │ 4   │
    │     │     │     │     │     │     │
────┴─────┴─────┴─────┴─────┴─────┴─────┴────

A reference like "C3" indicates a specific zone on the drawing.
This is useful for:
- Locating features during discussion
- Identifying drawing errors
- Cross-referencing between drawing sheets
```

## 4.5 Drawing Formats for Digital Environments

### 4.5.1 Electronic Drawing Formats

Modern technical drawing increasingly occurs in digital environments. Key considerations include:

**File Formats:**

| Format | Application | Features |
|--------|-------------|----------|
| PDF | Distribution, archival | Preserves formatting, searchable |
| DXF | CAD exchange | Geometry exchange between systems |
| DWG | Native CAD files | Full editability (proprietary) |
| STEP | 3D model exchange | 3D geometry transfer |
| SVG | Web, simple graphics | Scalable vector graphics |

**Standard Sheet Sizes for Digital Drawing:**

| Format | Pixel Dimensions (at 300 DPI) |
|--------|-------------------------------|
| A4 | 2480 × 3508 |
| A3 | 3508 × 4961 |
| A2 | 4961 × 7016 |
| A1 | 7016 × 9933 |
| A0 | 9933 × 14043 |

### 4.5.2 Margins for Digital Drawings

**Print Margin Requirements:**
- Bleed area: 3-5mm beyond trim marks
- Safe zone: 5mm inside trim marks for critical content
- Title block position: 10mm from right and bottom trim

## 4.6 Common Mistakes with Drawing Formats

### Mistake 1: Incorrect Margin Application

**Problem:** Title block extends beyond the drawing area or is too close to the edge.

**Correction:** Standardize margin sizes and verify before finalizing.

### Mistake 2: Missing Zone Marking

**Problem:** Drawing lacks zone references, making communication difficult.

**Correction:** Add zone markings when required by project standards.

### Mistake 3: Scale Not Indicated

**Problem:** Drawing contains no scale notation anywhere.

**Correction:** Always specify scale in title block; add local scale notation for detail views.

### Mistake 4: Inconsistent Sheet Size

**Problem:** Using mixed sheet sizes within one drawing set.

**Correction:** Establish sheet size standards and stick to them throughout the project.

## 4.7 References and Further Reading

- **ISO 5457:1999** — Technical product documentation — Sizes and layout of drawing sheets
- **ISO 7200:2004** — Technical product documentation — Title data fields
- **ISO 5455:1979** — Technical drawings — Scales
- **ASME Y14.1-2020** — Drawing Sheet Size and Format

---

# 5. Title Blocks and Drawing Identification

## 5.1 Advanced Title Block Design

### 5.1.1 Multi-Sheet Drawing Organization

When a drawing requires multiple sheets, the title block provides critical cross-referencing information.

**Sheet 1 (First Sheet) Contains:**
- Complete drawing title
- Full title block
- Bill of materials (if assembly)
- General notes
- Revision history

**Subsequent Sheets Contain:**
- Sheet-specific title (may be abbreviated)
- "SHEET X OF Y" notation
- Simplified title block
- Reference to first sheet for complete information

### 5.1.2 Example 5.1: Multi-Sheet Drawing System

```
SHEET 1 OF 3:
┌──────────────────────────────────────────────────────────────────┐
│  ACME CORP.                        DWG NO: AC-2024-0150          │
│  ┌────────┐                       SHEET 1 OF 3                 │
│  │  LOGO  │                                                    
│  └────────┘                                                    
│─────────────────────────────────────────────────────────────────│
│  TITLE: INDUSTRIAL GEARBOX ASSEMBLY                              │
│          MODEL GB-500                                            │
│─────────────────────────────────────────────────────────────────│
│  SCALE   │   DATE   │  DRAWN │  CHECKED │  APPROVED │  REV     │
│  1:10    │ 2024-04  │  M.Chen │ S.Liu   │  R.Patel  │ A        │
│─────────────────────────────────────────────────────────────────│
│                      BILL OF MATERIALS                           │
│  ────────────────────────────────────────────────────────────    │
│  ITEM │ QTY │ DESCRIPTION              │ DWG NO │ MATERIAL    │
│  ─────┼─────┼────────────────────────────┼────────┼─────────   │
│  1    │  1  │ Housing, main              │ 0151   │ GJS-400    │
│  2    │  1  │ Input shaft                │ 0152   │ 42CrMo4    │
│  3    │  2  │ Bearing, roller            │ ISO-RL │ See std.   │
│  ...  │     │                            │        │            │
│─────────────────────────────────────────────────────────────────│
│ NOTES:                                                            │
│ 1. ALL DIMENSIONS IN MM UNLESS OTHERWISE NOTED                   │
│ 2. GENERAL TOLERANCES: ISO 2768-m                                │
│ 3. BREAK ALL SHARP EDGES 0.2 MAX                                  │
└──────────────────────────────────────────────────────────────────┘

SHEET 2 OF 3:
┌──────────────────────────────────────────────────────────────────┐
│  ACME CORP.                        DWG NO: AC-2024-0150          │
│  ┌────────┐                       SHEET 2 OF 3                   │
│  │  LOGO  │                       (MAIN HOUSING)                  │
│  └────────┘                                                    
│─────────────────────────────────────────────────────────────────│
│  TITLE: GEARBOX - MAIN HOUSING                                   │
│─────────────────────────────────────────────────────────────────│
│  SCALE   │   DATE   │  DRAWN │  CHECKED │  APPROVED │  REV     │
│  1:2     │ 2024-04  │  M.Chen │ S.Liu   │  R.Patel  │ A        │
│─────────────────────────────────────────────────────────────────│
│                                                                 │
│              [DRAWING VIEWS HERE]                               │
│                                                                 │
│─────────────────────────────────────────────────────────────────│
│  SEE SHEET 1 FOR NOTES, BOM, AND APPROVAL INFORMATION          │
└──────────────────────────────────────────────────────────────────┘
```

## 5.2 Drawing Numbering Systems

### 5.2.1 Common Numbering Schemes

**Alphanumeric System:**
```
Structure: XX-YYYY-NNN
XX = Department code (DE, ME, EE, etc.)
YYYY = Project or product number
NNN = Sequential drawing number

Example: ME-2024-0145
ME = Mechanical Engineering
2024 = Year of origin
0145 = Drawing sequence number
```

**Hierarchical System:**
```
Structure: A.B.C.D.E
A = Major assembly level (0 = top assembly)
B = Sub-assembly level
C = Part within sub-assembly
D = Detail feature (if needed)
E = Revision

Example: 1.3.2.0.A
1 = Product family
3 = Sub-assembly third in sequence
2 = Part second in sub-assembly
0 = Part itself (no further detail)
A = Revision A
```

### 5.2.2 Example 5.2: Establishing a Drawing Numbering System

```
COMPANY: MidSize Manufacturing Co.

REQUIREMENTS:
- Track 5 product lines
- Support 3 levels of assembly
- Maintain revision history
- Enable cross-referencing

PROPOSED SYSTEM: PR-LL-AAAA-NNN-R

Where:
PR   = Product code (2 alphanumeric)
LL   = Drawing level (01=assembly, 02=sub-assembly, 03=detail)
AAAA = Sequential number (0001-9999)
NNN  = Optional sheet number (001-999, default 001)
R    = Revision (A-Z)

EXAMPLES:
MS01-010001-001-A = Pump Assembly, Rev A, Sheet 1
MS01-020012-001-B = Pump Sub-assembly 12, Rev B, Sheet 1
MS01-030123-001-A = Bearing Cap Detail, Rev A, Sheet 1

ADVANTAGES:
✓ Clear hierarchy identification
✓ Automatic sheet sequencing
✓ Revision tracking built-in
✓ Scalable to any product complexity
```

## 5.3 Revision Control

### 5.3.1 Revision Block Design

The revision block documents the history of changes to a drawing.

**Standard Revision Block Fields:**

| Field | Content | Format |
|-------|---------|--------|
| Rev | Revision identifier | Letter (A, B, C...) or Number (1, 2, 3...) |
| Date | Date of revision | YYYY-MM-DD |
| Description | Nature of change | Text description |
| Approved | Authority for change | Name or initials |

### 5.3.2 Revision Block Example

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                   │
│  REVISION HISTORY                                                 │
│  ─────────────────                                                 │
│  ────────────────────────────────────────────────────────────── │
│  REV │   DATE   │  DESCRIPTION                       │ APPROVED │
│  ────┼──────────┼────────────────────────────────────┼───────── │
│  A   │ 2024-01  │ Initial release                     │ J.Smith │
│  B   │ 2024-03  │ Added detail D, changed tolerance   │ J.Smith │
│  C   │ 2024-05  │ Material change S355 to S420        │ K.Lee   │
│  ────┴──────────┴────────────────────────────────────┴───────── │
│                                                                   │
└─────────────────────────────────────────────────────────────────┘
```

### 5.3.3 Change Management Best Practices

**Rule 1: Never Erase or White-Out**
Changes to official drawings must be traceable. Use revision marks and update the revision block.

**Rule 2: Describe Changes Clearly**
A good change description answers:
- What changed? (e.g., "Hole diameter increased")
- Why it changed? (e.g., "To accommodate larger fastener")
- What else might be affected? (e.g., "See detail B")

**Rule 3: Maintain Revision Hierarchy**
Higher-level assembly drawings must be revised when subordinate drawings change.

**Example 5.3: Revision Management Scenario**

```
ORIGINAL DRAWING (Rev A):
- Housing bore diameter: Ø50.00 ± 0.05mm
- Bearing selected: SKF 6210

ENGINEERING CHANGE REQUEST:
- Customer requires increased load capacity
- Solution: Increase bore to Ø55.00, select larger bearing

REVISION PROCESS:

Step 1: Update detail drawing (housing)
- New dimension: Ø55.00 ± 0.05mm
- Update Rev A → Rev B
- Update revision description: "Bore increased Ø50 to Ø55"

Step 2: Update sub-assembly drawing
- Change bearing selection from 6210 to 6211
- Update Rev A → Rev B
- Update reference to housing drawing

Step 3: Update top-level assembly drawing
- Update bill of materials
- Update Rev A → Rev B
- Note: "Refer to sheet 2 for bearing change"

Step 4: Issue ECN (Engineering Change Notice)
- Document reason for change
- Identify affected documents
- Set effective date
- Distribute to stakeholders
```

## 5.4 References and Further Reading

- **ISO 128-1:2020** — Presentation of views
- **ASME Y14.35M-1997** — Revision of Engineering Drawings and Associated Documents
- **Mil-Standard 100** — Department of Defense Standard Practice for Engineering Drawings

---

# 6. Types of Technical Drawings

## 6.1 Assembly Drawings

An **assembly drawing** shows how individual parts are arranged, connected, and identified within a complete product or sub-assembly. It is one of the most important documents in manufacturing, quality control, and maintenance.

### 6.1.1 Purpose of Assembly Drawings

Assembly drawings serve multiple critical functions:

1. **Manufacturing Guidance:** Shows how parts fit together during assembly
2. **Quality Control:** Enables inspection of assembled products
3. **Maintenance:** Guides repair and overhaul procedures
4. **Communication:** Provides a common reference for all stakeholders
5. **Documentation:** Creates a legal record of product configuration

### 6.1.2 Types of Assembly Drawings

| Type | Description | Application |
|------|-------------|-------------|
| General assembly | Shows complete product | Initial design, customer approval |
| Detail assembly | Detailed view of sub-section | Complex areas, clarification |
| Installation assembly | Shows product in context | Building in, plant layout |
| Transport assembly | Shipping configuration | Packaging, logistics |
| Explosive view | Parts separated for clarity | Parts identification, manuals |

### 6.1.3 Essential Elements of Assembly Drawings

**Example 6.1: Complete Assembly Drawing Requirements**

```
ASSEMBLY DRAWING CHECKLIST:

[✓] Drawing Views
    ├── Required orthographic views (front, top, side)
    ├── Section views showing internal features
    ├── Detail views for complex areas
    └── Special views (exploded, enlarged)

[✓] Identification
    ├── Part numbers in balloons
    ├── Leader lines with dots at part
    ├── Parts list (Bill of Materials)
    └── Reference designations

[✓] Connection Information
    ├── Fastener specifications
    ├── Tightening sequences (if critical)
    ├── Torque specifications
    └── Adhesive/locking specifications

[✓] Functional Information
    ├── Critical dimensions (fits, clearances)
    ├── Adjustment points
    ├── Range of motion indicators
    └── Performance specifications

[✓] Documentation
    ├── Title block complete
    ├── Revision block updated
    ├── Notes and specifications
    └── Approval signatures
```

### 6.1.4 Bill of Materials (BOM)

The Bill of Materials (also called Parts List or Schedule) is an integral part of every assembly drawing.

**BOM Structure:**

| Column | Content | Example |
|--------|---------|---------|
| Item | Sequential number | 1, 2, 3... |
| Part No. | Unique identifier | HB-M8-40-SS |
| Qty | Quantity per assembly | 4 |
| Description | Part name | Hex bolt M8×40 |
| Material | Material designation | A2-70 stainless |
| Surface treatment | Finish specification | Passivated |
| Remarks | Additional information | Standard part |

**Example 6.2: Bill of Materials**

```
┌─────────────────────────────────────────────────────────────────────┐
│                         BILL OF MATERIALS                            │
│                     PUMP ASSEMBLY, MODEL P-200                       │
├──────┬──────────────┬─────┬────────────────────┬──────────┬─────────┤
│ ITEM │  PART NO.    │ QTY │   DESCRIPTION      │ MATERIAL │ REMARKS │
├──────┼──────────────┼─────┼────────────────────┼──────────┼─────────┤
│  1   │ P200-001     │  1  │ Pump housing       │ Cast iron│ Machined│
│  2   │ P200-002     │  1  │ Impeller           │ Bronze   │ Balanced│
│  3   │ P200-003     │  1  │ Shaft              │ SS 316   │ Hardened│
│  4   │ P200-004     │  2  │ Bearing 6208       │ Steel    │ Standard│
│  5   │ P200-005     │  1  │ Seal assembly      │ NBR      │ Replace │
│  6   │ HB-M8-40-SS  │  8  │ Hex bolt M8×40     │ A2-70 SS │ Standard│
│  7   │ HN-M8-SS     │  8  │ Hex nut M8         │ A2-70 SS │ Standard│
│  8   │ LW-8-SS      │  8  │ Lock washer M8     │ A2 SS    │ Standard│
│  9   │ P200-009     │  1  │ Cover plate        │ Cast iron│ Machined│
│ 10   │ P200-010     │  1  │ Gasket             │ Cork     │ Replace │
└──────┴──────────────┴─────┴────────────────────┴──────────┴─────────┘
│                                                                       │
│ NOTES:                                                                │
│ 1. All fasteners to be tightened to 25 Nm torque                     │
│ 2. Apply thread-locking compound to items 6 and 7                    │
│ 3. Replace items 5 and 10 during each overhaul                       │
│ 4. Bearing preload: 0.02mm                                            │
└─────────────────────────────────────────────────────────────────────┘
```

### 6.1.5 Balloon Callouts and Leader Lines

**Balloon Standards:**
- Circular balloons with item numbers
- Leader lines with arrowheads or dots
- Avoid crossing leader lines when possible
- Place balloons outside the part outline

**Example 6.3: Balloon Placement Best Practices**

```
GOOD PRACTICE:                    POOR PRACTICE:
                                  
    ┌───┐                             ┌───┐
    │ 1 │───────►                     │ 1 │
    └───┘                             └─┬─┘
                                        │
    ┌───┐                               ▼
    │ 2 │───────►                   ┌───────┐
    └───┘                           │       │
                                    │   ┌───┼───┐
    ┌───┐                           │   │ 2 │   │
    │ 3 │───────►                   │   └───┘   │
    └───┘                           │           │
                                    └───────────┘
Clear, organized                   Cluttered, confusing
No crossing lines                  Lines cross part
```

## 6.2 Detail Drawings

A **detail drawing** (also called **part drawing** or **component drawing**) provides complete information for manufacturing a single part. Unlike assembly drawings that show relationships between parts, detail drawings focus on one component with all necessary dimensions, tolerances, materials, and manufacturing specifications.

### 6.2.1 Essential Elements of Detail Drawings

**Complete Detail Drawing Requirements:**

1. **Geometric Information**
   - All necessary orthographic views
   - Section views for internal features
   - Detail views for small features
   - Auxiliary views for inclined surfaces

2. **Dimensional Information**
   - All dimensions required for manufacture
   - Geometric tolerances (GD&T)
   - Surface finish specifications
   - Critical dimensions highlighted

3. **Material Specifications**
   - Material designation (e.g., AISI 1045, Al 6061-T6)
   - Heat treatment requirements
   - Hardness specifications
   - Material certifications required

4. **Manufacturing Information**
   - Surface finish symbols
   - Machining notes
   - Welding symbols (if applicable)
   - Special processes (plating, coating, etc.)

**Example 6.4: Detail Drawing Checklist**

```
DETAIL DRAWING VERIFICATION:

[✓] Views and Projections
    ├── Sufficient views to define all features
    ├── Section views for internal geometry
    ├── Detail views for complex areas
    └── Projection system indicated

[✓] Dimensions
    ├── All manufacturing dimensions present
    ├── No missing dimensions
    ├── No duplicate dimensions
    ├── Dimensions placed on appropriate views
    └── Tolerance specifications complete

[✓] Material and Treatment
    ├── Material specification complete
    ├── Heat treatment specified (if required)
    ├── Surface treatment specified (if required)
    └── Hardness requirements stated

[✓] Manufacturing Notes
    ├── Surface finish symbols applied
    ├── Special processes noted
    ├── Inspection requirements stated
    └── Quality standards referenced

[✓] Documentation
    ├── Title block complete
    ├── Part number assigned
    ├── Revision level current
    └── Approval signatures present
```

### 6.2.2 Dimensioning Hierarchy

Dimensions on detail drawings should follow a logical hierarchy:

| Priority | Type | Purpose | Example |
|----------|------|---------|---------|
| 1 | Functional | Critical to part function | Bearing bore diameter |
| 2 | Mating | Required for assembly | Bolt hole locations |
| 3 | Manufacturing | Needed for production | Stock size, rough dimensions |
| 4 | Reference | For information only | Overall length (REF) |

## 6.3 Schematic Drawings

**Schematic drawings** use simplified symbols to represent components and their relationships, focusing on function rather than physical appearance. Common types include:

### 6.3.1 Types of Schematic Drawings

| Type | Application | Key Features |
|------|-------------|--------------|
| Electrical | Circuits, wiring | Standard electrical symbols |
| Hydraulic | Fluid power systems | ISO 1219 symbols |
| Pneumatic | Compressed air systems | ISO 1219 symbols |
| Piping & Instrumentation (P&ID) | Process systems | ISA symbols |
| Logic diagrams | Control systems | Boolean logic symbols |

### 6.3.2 Schematic Drawing Principles

**Key Principles:**
1. **Functional arrangement** over physical layout
2. **Standard symbols** for all components
3. **Clear signal flow** (left to right, top to bottom)
4. **Component identification** with reference designators
5. **Connection clarity** with line routing

**Example 6.5: Hydraulic Schematic Symbols**

```
COMMON HYDRAULIC SYMBOLS:

Pump (fixed displacement):     ──►◄──
Pump (variable displacement):  ──►◄── with diagonal arrow
Motor (hydraulic):             ──►M◄──
Cylinder (single-acting):      ├──┤
Cylinder (double-acting):      ├──┼──┤
Directional valve (4/3):       ┌─┬─┐
                               │ │ │
                               └─┴─┘
Pressure relief valve:         ──┤├──
Check valve:                   ──►├──
Filter:                        ──◊──
Reservoir:                     ┌───┐
                               │   │
                               └───┘
```

## 6.4 Installation Drawings

**Installation drawings** show how a product is to be installed in its operating environment, including:

- Foundation requirements
- Clearance dimensions
- Utility connections
- Access requirements
- Environmental considerations

### 6.4.1 Installation Drawing Content

**Typical Information Included:**

```
INSTALLATION DRAWING ELEMENTS:

1. LOCATION INFORMATION
   ├── Overall dimensions
   ├── Mounting points
   ├── Foundation details
   └── Clearance requirements

2. CONNECTION INFORMATION
   ├── Electrical connections
   ├── Piping connections
   ├── Ductwork connections
   └── Control wiring

3. ACCESS REQUIREMENTS
   ├── Maintenance clearances
   ├── Service access points
   ├── Removal paths
   └── Safety zones

4. ENVIRONMENTAL DATA
   ├── Operating temperature range
   ├── Humidity limits
   ├── Vibration isolation
   └── Noise considerations
```

## 6.5 References and Further Reading

- **ISO 128-30:2001** — Technical drawings — General principles of representation — Part 30: Basic conventions for views
- **ISO 1219-1:2012** — Fluid power systems and components — Graphic symbols and circuit diagrams
- **ASME Y14.24-2012** — Types and Applications of Engineering Drawings
- **IEEE 315-1975** — Graphic Symbols for Electrical and Electronics Diagrams

---

# 7. Special Drawing Representations

## 7.1 Simplified Representations

To improve drawing clarity and reduce drafting time, standards allow **simplified representations** for common features. These conventions are universally recognized and eliminate the need for complete geometric detail in certain situations.

### 7.1.1 Repetitive Features

When a part has multiple identical features (holes, slots, etc.), they can be represented in simplified form.

**Example 7.1: Bolt Circle Representation**

```
FULL REPRESENTATION:          SIMPLIFIED REPRESENTATION:

    ○     ○     ○                      ○
  ○           ○                    8× ○ EQ SP
○               ○                  ON Ø120 B.C.
  ○           ○
    ○     ○     ○

(8 holes drawn)              (1 hole drawn + note)

ADVANTAGES OF SIMPLIFIED:
✓ Faster to draw
✓ Clearer intent
✓ Easier to modify
✓ Less cluttered
```

### 7.1.2 Standard Parts

Standard parts (bolts, nuts, washers, bearings, etc.) can be represented in simplified form since their detailed geometry is defined by standards.

**Simplified Representations:**

| Component | Full Detail | Simplified |
|-----------|-------------|------------|
| Hex bolt | Complete threads, chamfers | Solid shaft with hex head |
| Hex nut | Complete threads, chamfers | Hexagon with center hole |
| Washer | Exact thickness, chamfers | Thin circle |
| Bearing | Balls, races, seals | Two concentric circles |
| Spring | All coils drawn | End coils + center line |

**Example 7.2: Bolt Assembly Simplification**

```
FULL DETAIL:                 SIMPLIFIED:

┌─────────┐                  ┌─────────┐
│  ╱╲╱╲╱  │                  │  ▄▄▄▄▄  │
│ ╱  ╲  ╲ │                  │  █████  │
├─────────┤                  ├─────────┤
│ ▓▓▓▓▓▓▓ │                  │ ▓▓▓▓▓▓▓ │
│ ▓▓▓▓▓▓▓ │                  │ ▓▓▓▓▓▓▓ │
│ ▓▓▓▓▓▓▓ │                  │ ▓▓▓▓▓▓▓ │
│ ▓▓▓▓▓▓▓ │                  │ ▓▓▓▓▓▓▓ │
│ ▓▓▓▓▓▓▓ │                  │ ▓▓▓▓▓▓▓ │
└─────────┘                  └─────────┘

Threads shown              Threads implied
Time: 10 minutes          Time: 2 minutes
```

### 7.1.3 Symmetrical Parts

For symmetrical parts, only half (or a quarter) of the part needs to be drawn, with a centerline indicating the axis of symmetry.

**Example 7.3: Half-Section of Symmetrical Shaft**

```
FULL DRAWING:                HALF-SECTION:

┌─────────────────┐          ┌─────────────────┐
│                 │          │▓▓▓▓▓▓▓▓▓│       │
│                 │          │▓▓▓▓▓▓▓▓▓│       │
│                 │          ├─────────┼───────┤ ← Centerline
│                 │          │         │       │
│                 │          │         │       │
└─────────────────┘          └─────────────────┘

Shows external only        Shows internal & external
                          in one view
```

## 7.2 Conventional Breaks

**Conventional breaks** are used to shorten the representation of long, uniform parts (shafts, tubes, bars) without losing essential information.

### 7.2.1 Break Line Types

| Material | Break Line Style | Application |
|----------|------------------|-------------|
| Solid round | Wavy line with solid ends | Shafts, rods |
| Hollow round | Wavy line with hollow ends | Pipes, tubes |
| Rectangular | Zigzag line | Bars, plates |
| Wood | Irregular jagged line | Timber, lumber |

**Example 7.4: Shaft with Conventional Break**

```
WITHOUT BREAK:
├──────────────────────────────────────────────────────────────┤
│                                                              │
│                        500mm                                 │
│                                                              │
└──────────────────────────────────────────────────────────────┘

WITH BREAK:
├──────────┤  ╱╲╱╲  ├──────────┤
│          │  ╲╱╲╱  │          │
│   50mm   │        │   50mm   │
│          │        │          │
└──────────┘        └──────────┘
            500mm (total length noted)

ADVANTAGES:
✓ Saves drawing space
✓ Allows larger scale for details
✓ Maintains dimensional information
```

## 7.3 Partial Views

When a view would be largely repetitive or symmetrical, a **partial view** shows only the necessary portion.

### 7.3.1 When to Use Partial Views

**Appropriate situations:**
- Symmetrical parts (show half)
- Repetitive patterns (show one repeat)
- Large parts with local features (show feature area)
- Identical sections (show one section)

**Example 7.5: Partial View of Flange**

```
FULL VIEW:                   PARTIAL VIEW:

    ○   ○   ○   ○                ○   ○
  ○               ○            ○       ○
○                   ○        ○           ○
│                   │        │           │
○                   ○        ├───────────┤
  ○               ○          │           │
    ○   ○   ○   ○            │           │
                             └───────────┘
                                  │
                             Centerline
                             (symmetry implied)
```

## 7.4 Removed Sections

A **removed section** is a cross-sectional view that is drawn separately from the main view, typically at a larger scale to show detail.

### 7.4.1 Removed Section Conventions

**Key elements:**
1. **Cutting plane line** on main view
2. **Section identification** (A-A, B-B, etc.)
3. **Viewing direction arrows**
4. **Separate section view** with label
5. **Scale notation** (if different from main view)

**Example 7.6: Removed Sections of I-Beam**

```
MAIN VIEW:                    REMOVED SECTIONS:

    A                         SECTION A-A
    │                         ┌─────────┐
    ▼                         │         │
┌───┴───┐                     ├─────────┤
│       │                     │         │
│       │  ◄── B              │         │
│       │      │              │         │
│       │      ▼              ├─────────┤
│       │  ┌───┴───┐          │         │
│       │  │       │          └─────────┘
│       │  │       │
│       │  │       │          SECTION B-B
│       │  │       │          ┌───────────┐
│       │  │       │          │           │
│       │  └───────┘          │           │
│       │                     │           │
└───────┘                     │           │
                              │           │
                              └───────────┘
                              
                              Scale: 2:1
```

## 7.5 Developed Views (Flat Patterns)

For sheet metal parts, a **developed view** shows the part "unfolded" to its flat pattern before bending.

### 7.5.1 Bend Allowance Calculations

When sheet metal is bent, the neutral axis stretches. The **bend allowance** accounts for this:

```
BEND ALLOWANCE FORMULA:

BA = (π/180) × R × A × (K-factor)

Where:
BA = Bend allowance
R = Inside bend radius
A = Bend angle (degrees)
K = K-factor (material-dependent, typically 0.33-0.50)

EXAMPLE:
Material: 2mm steel
Inside radius: 3mm
Bend angle: 90°
K-factor: 0.4

Calculation:
BA = (pi/180) x R x A x K
BA = (3.1416/180) x 3 x 90 x 0.4
BA = 1.885 mm

Use this value when preparing the flat pattern length.
```

### 7.5.2 Practical Flat Pattern Example

Given a U-bracket with two 90 degree bends:
- Leg 1: 40 mm
- Base: 30 mm
- Leg 2: 40 mm
- Thickness: 2 mm
- Inside bend radius: 3 mm
- K-factor: 0.4

Steps:
1. Compute bend allowance per bend (from above): 1.885 mm.
2. Two bends give total bend allowance: 3.77 mm.
3. Flat length = 40 + 30 + 40 + 3.77 = 113.77 mm.
4. Round to manufacturing precision (for example 113.8 mm).

Notes:
- Some shops use bend deduction tables instead of direct formulas.
- Always validate first-piece production against actual formed geometry.

## 7.6 Moved and Local Views

Moved views are placed away from strict projection alignment to improve readability.
Local views show only a selected region and are often bounded by freehand lines.

When using them:
1. Keep view labels clear (for example View C, Detail D).
2. Add arrows indicating viewing direction.
3. Preserve scale notation for each local/moved view.
4. Avoid ambiguity with leader lines and references.

## 7.7 References and Further Reading

- ISO 128-30: General principles of representation
- ISO 5456 series: Projection methods
- ASME Y14.3: Multiview and sectional view drawings

---

# 8. Sections and Cuts

## 8.1 Why Sections Are Required

Hidden lines alone are often insufficient for complex internal geometry. Sections expose interior features cleanly.

## 8.2 Basic Procedure

1. Define a cutting plane.
2. Remove the material between observer and cutting plane.
3. Draw the remaining geometry.
4. Hatch cut material with thin, evenly spaced lines.

## 8.3 Hatching Rules

- Use thin continuous lines.
- Keep spacing consistent for the same part region.
- Do not hatch through dimension text or symbols.
- Adjacent parts in assembly sections should use different hatch directions or spacing.

## 8.4 Common Section Types

| Type | Use Case | Note |
|------|----------|------|
| Full section | Entire object internal view | Most common for single parts |
| Half section | Symmetrical objects | One half exterior, one half section |
| Local section | Small internal area only | Bounded by freehand break line |
| Offset section | Features on different planes | Cutting plane jogs through key features |
| Aligned section | Angled features | Rotated into plane for representation |

## 8.5 Worked Example: Half Section on a Flanged Hub

Input:
- Hub outer diameter: 80 mm
- Bore: 30 mm
- Flange thickness: 10 mm
- Body length: 50 mm

Output logic:
1. Draw centerline axis.
2. Right half: external view with visible outlines.
3. Left half: sectioned interior with hatching on solid material only.
4. Leave bore area unhatched.

Typical beginner error:
- Hatching the hole area. Holes are voids and remain blank.

## 8.6 Exceptions and Conventions

- Do not hatch shafts, fasteners, keys, and thin ribs when cut along their longitudinal axis in assembly sections.
- Do not draw hidden lines in a section unless needed for clarity.

## 8.7 References

- ISO 128-40 to 128-50 (sectional representation)
- ASME Y14.3 and Y14.5

---

# 9. Threads and Threaded Components

## 9.1 External and Internal Thread Representation

- External thread major diameter: thick line.
- External thread minor diameter: thin line.
- Internal thread major diameter: thin line.
- Internal thread minor diameter: thick line.

## 9.2 Standard Thread Callouts

Format examples:
- M16 x 2
- M12 x 1.75 - 6g (external)
- M12 x 1.75 - 6H (internal)

Rules:
1. Use M for metric ISO threads.
2. Include pitch if non-coarse or if explicit requirement exists.
3. Add tolerance class when functionally required.

## 9.3 Blind Tapped Hole Example

Specification:
- Thread: M10 x 1.5
- Thread depth: 18 mm
- Drill depth: 22 mm
- Drill point angle: 120 deg

Recommended callout:
M10 x 1.5 - 6H, 18 DEEP
DRILL 8.5, 22 DEEP

## 9.4 Assembly Priority Rule

In screw-in-hole assemblies, conventionally represent mating thread engagement clearly, with the fastener representation taking precedence in simplified assembly views.

## 9.5 Common Errors

- Using diameter symbol with metric thread callout (avoid in thread designation itself).
- Omitting depth for blind holes.
- Confusing drill diameter and nominal thread diameter.

---

# 10. Fastening Assemblies

## 10.1 Screw Joint vs Bolt-Nut Joint

Screw joint:
- Screw threads directly into one part.
- Clamp force is under screw head and mating thread.

Bolt-nut joint:
- Bolt passes through both parts.
- Clamp force is under bolt head and nut.

## 10.2 Washer Use Cases

- Spread bearing load.
- Protect softer surfaces.
- Improve locking behavior when paired with lock washers or prevailing torque nuts.

## 10.3 Worked Design Example

Given:
- Two steel plates, total clamped thickness: 18 mm
- Required preload class: medium
- Preferred thread: M8

Quick selection:
1. Choose bolt length covering grip + washer + nut engagement.
2. Practical pick: M8 x 30.
3. Add flat washer both sides for slot protection if needed.
4. Define tightening torque per property class and lubrication condition.

## 10.4 Drawing Notes Template

- FASTENERS ISO 4017 M8 x 30, PROPERTY CLASS 8.8, Zn PLATED
- NUTS ISO 4032 M8, CLASS 8
- TORQUE TO 24 N.m DRY

---

# 11. Dimensioning Rules and Best Practices

## 11.1 Core Principles

1. Dimension only what is necessary.
2. Avoid duplicate dimensions.
3. Dimension from functional datums when possible.
4. Keep dimensions outside view boundaries when practical.
5. Do not dimension to hidden lines.

## 11.2 Functional Dimensioning Strategy

Order dimensions by intent:
- Primary functional interfaces
- Assembly interfaces
- Manufacturing convenience dimensions
- Reference dimensions

## 11.3 Example: Hole Pattern Dimensioning

Bad pattern:
- Chain dimensions between adjacent holes only.

Better pattern:
1. Set datum A (base), datum B (side).
2. Locate each hole from A and B.
3. Add diameter and positional tolerance.

Sample callout:
4X DIA 8 THRU
POS 0.10 A B

## 11.4 Tolerances

Types:
- Limit dimensions
- Plus/minus tolerances
- General tolerance standards
- Geometric tolerances (GD&T)

Example:
50.00 +/- 0.05

## 11.5 Typical Mistakes

- Over-dimensioning the same feature in multiple views.
- Mixing inch and mm unintentionally.
- Missing units note in title block.

---

# 12. Cavalier and Cabinet Perspectives

## 12.1 Quick Comparison

| Method | Receding Scale | Typical Use |
|--------|----------------|-------------|
| Cavalier | Full scale (k = 1) or reduced by choice | Fast conceptual communication |
| Cabinet | Half scale (k = 0.5) | More realistic proportion |

## 12.2 Construction Steps

1. Draw front face true shape.
2. Choose receding axis angle (commonly 30, 45, or 60 deg).
3. Apply receding scale factor k.
4. Complete rear edges and visible outlines.

## 12.3 Example

Block 60 x 40 x 30 mm, cabinet projection:
- Front rectangle: 60 x 40.
- Receding depth plotted as 30 x 0.5 = 15 mm.
- Connect corners along receding axis.

---

# 13. Surface Intersections

## 13.1 Method Overview

To find intersection curves between surfaces:
1. Mark extreme points.
2. Use auxiliary cutting planes.
3. Find intersection points on each surface.
4. Transfer points between views.
5. Draw smooth visible/hidden intersection curves.

## 13.2 Cylinder-Cylinder Example

Given:
- Main cylinder: dia 80
- Branch cylinder: dia 50 at 90 deg

Procedure:
1. Divide branch circle in top view into equal points.
2. Project each point onto main cylinder generators.
3. Locate corresponding heights in front view.
4. Connect points with smooth curve.

Tip:
- Use symmetry; only half the curve may need construction.

---

# 14. The Technical Drawing Process

## 14.1 End-to-End Workflow

1. Analyze function and interfaces.
2. Choose projection method and primary view.
3. Block layout on sheet.
4. Add major geometry and centerlines.
5. Add secondary features.
6. Create sections/details where needed.
7. Add dimensions and tolerances.
8. Add notes, title block, revision.
9. Perform final quality check.

## 14.2 Quality Checklist

- Are all required views present?
- Are dimensions complete and non-redundant?
- Are line types consistent?
- Is the projection method marked?
- Are tolerances and finishes specified?
- Is revision state current?

## 14.3 Time Management for Manual Drafting

- First 20% time: layout and strategy.
- Middle 60%: geometry and projection.
- Final 20%: dimensions, verification, cleanup.

---

# 15. Assembly Plan Interpretation

## 15.1 Reading Sequence

1. Read title block and revision.
2. Inspect BOM and item balloons.
3. Identify fixed vs moving groups.
4. Verify fits, clearances, and constraints.
5. Interpret sections for hidden interfaces.

## 15.2 Mechanism Clues from Standard Parts

- Bearing or bushing: likely pivot or rotating support.
- Key: torque transmission with removable connection.
- Circlip: axial retention.
- Spring: preload or return force.

## 15.3 Example Interpretation Snapshot

If you see shaft + key + gear + two bearings:
- Likely a rotating transmission stage.
- Bearings constrain radial position.
- Circlip or shoulder controls axial movement.
- Key transmits torque from shaft to gear hub.

---

# 16. Standardized Fastening Elements

## 16.1 Screws

Common families:
- Hex head screw (ISO 4014/4017)
- Socket head cap screw (ISO 4762)
- Set screw/headless screw (ISO 4026/4027)

Designation examples:
- HEX SCREW ISO 4017 M8 x 40 - 8.8
- SHCS ISO 4762 M12 x 70 - 12.9

## 16.2 Nuts and Washers

- Hex nut ISO 4032
- Prevailing torque nut (nylon insert) ISO 7040 variants
- Flat washer ISO 7089/7090
- Spring lock washer (where specified by organization standard)

## 16.3 Retaining and Pin Elements

- External circlip DIN 471
- Internal circlip DIN 472
- Spring pin ISO 8752

## 16.4 Selection Considerations

1. Mechanical load and fatigue.
2. Corrosion environment.
3. Serviceability and assembly tools.
4. Standard availability and cost.

---

# 17. Technical Terminology and Definitions

## 17.1 Geometry Terms

- Through hole: hole passing completely through material.
- Blind hole: hole with finite depth, closed at one end.
- Counterbore: cylindrical recess to seat screw head.
- Countersink: conical recess, usually for flat head screws.
- Chamfer: beveled edge.
- Fillet: rounded internal corner.
- Round: rounded external corner.
- Boss: raised cylindrical or prismatic feature.
- Rib: thin strengthening wall.

## 17.2 Fit and Tolerance Terms

- Clearance fit: always positive clearance.
- Transition fit: possible small clearance or interference.
- Interference fit: always overlap requiring press/shrink assembly.
- Datum: theoretically exact reference feature for measurement.

## 17.3 Surface and Process Terms

- Ra: arithmetic mean roughness.
- Machining allowance: extra stock for final machining.
- Heat treatment: thermal process to modify properties.
- Deburring: removing sharp edges and burrs.

---

# 18. Appendices and Reference Materials

## 18.1 Quick Study Summary

- Orthographic views are the base language of technical drawing.
- Line types communicate visibility and function.
- Sections reveal internal geometry efficiently.
- Dimensioning must be complete, non-redundant, and functional.
- Thread and fastener conventions prevent ambiguity.
- Standards ensure cross-team and cross-country consistency.

## 18.2 Practical Self-Check Before Releasing a Drawing

1. Could a machinist build the part without asking questions?
2. Are all interfaces and fits fully defined?
3. Is every critical requirement verifiable by inspection?
4. Are notes and standards references consistent?
5. Is revision and approval status updated?

## 18.3 Practice Problems with Short Answers

Problem 1:
Create minimum views for a stepped shaft with cross-hole.
Short answer: front + side + section through cross-hole.

Problem 2:
A blind tapped hole reads M8 x 1.25, 12 deep. Which diameter is used to drill?
Short answer: tapping drill close to 6.8 mm (check standard drill chart).

Problem 3:
When should half-section be used?
Short answer: symmetric parts where interior and exterior can be shown in one view.

## 18.4 Recommended Standards Set

- ISO 128 (representation and line conventions)
- ISO 5455 (scales)
- ISO 5457 (sheet formats)
- ISO 7200 (title blocks)
- ISO 1101 (GPS/GD&T)
- ASME Y14.5 (dimensioning and tolerancing)

## 18.5 Suggested Learning Path

1. Master projection and line types.
2. Practice sections and hidden-feature interpretation.
3. Learn functional dimensioning with datum strategy.
4. Add GD&T and fit system proficiency.
5. Apply standards on real assemblies and peer review.

## 18.6 Closing Note

Technical drawing is not only a drafting skill; it is an engineering communication discipline. High-quality drawings reduce manufacturing errors, shorten lead times, and preserve design intent across the full product lifecycle.

---

End of document.
