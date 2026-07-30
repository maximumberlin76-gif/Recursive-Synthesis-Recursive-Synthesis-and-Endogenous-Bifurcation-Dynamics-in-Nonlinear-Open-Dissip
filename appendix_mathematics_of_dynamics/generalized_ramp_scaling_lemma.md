# Generalized Ramp-Scaling Lemma

This appendix states and proves the ramp-scaling law for the generalized critical normal form used in the Recursive Synthesis and Endogenous Bifurcation Dynamics framework.

The result separates the temporal critical exponent from the amplitude exponent and separates the algebraic scaling proof from any model-specific closure used to select the saturation order.

# Lemma Statement

Consider the generalized nonautonomous critical dynamics:

`dC/dt = v_eff t C − gC^n`

with:

- `v_eff > 0` — effective linear ramp velocity;
- `g > 0` — saturation coefficient;
- `n > 1` — saturation order;
- `C(t)` — reduced critical coherence amplitude.

Assume that the control parameter crosses the local critical region through the linear ramp term `v_eff t C` and that `gC^n` is the leading nonlinear saturation term in the analyzed regime.

Then the parameter-removing rescaling is:

`t = v_eff^(−1/2) τ`

`C = g^(−1/(n−1)) v_eff^(1/(2(n−1))) y`

and the dynamics reduce to:

`dy/dτ = τy − y^n`

Consequently:

`t_critical ~ v_eff^(−1/2)`

`t_delay ~ v_eff^(−1/2)`

and:

`C_critical ~ g^(−1/(n−1)) v_eff^(1/(2(n−1)))`

The temporal exponent `−1/2` is independent of `n` within this linear-ramp class. The amplitude exponent depends on `n`.

# Proof by Exponent Balance

Introduce the general scaling ansatz:

`t = v_eff^(−α) τ`

`C = g^(−1/(n−1)) v_eff^β y`

The derivative scales as:

`dC/dt ~ g^(−1/(n−1)) v_eff^(β+α) dy/dτ`

The linear ramp term scales as:

`v_eff t C ~ g^(−1/(n−1)) v_eff^(1−α+β) τy`

The nonlinear saturation term scales as:

`gC^n ~ g^(−1/(n−1)) v_eff^(nβ) y^n`

Parameter removal requires the three powers of `v_eff` to be equal:

`β + α = 1 − α + β = nβ`

From:

`β + α = 1 − α + β`

we obtain:

`2α = 1`

and therefore:

`α = 1/2`

From:

`β + α = nβ`

we obtain:

`α = (n−1)β`

and therefore:

`β = 1/(2(n−1))`

Substitution gives:

`t = v_eff^(−1/2) τ`

`C = g^(−1/(n−1)) v_eff^(1/(2(n−1))) y`

Every term then carries the common prefactor:

`g^(−1/(n−1)) v_eff^(1/2 + 1/(2(n−1)))`

After division by this prefactor, the reduced equation is:

`dy/dτ = τy − y^n`

This proves the stated temporal and amplitude scaling laws.

# Temporal and Amplitude Exponents

The lemma produces two distinct scaling statements.

Temporal scaling:

`t_critical ~ v_eff^(−1/2)`

`t_delay ~ v_eff^(−1/2)`

Amplitude scaling:

`C_critical ~ g^(−1/(n−1)) v_eff^(1/(2(n−1)))`

The temporal exponent is fixed by balancing the time derivative against the linear ramp term. It does not depend on the saturation order `n`.

The amplitude exponent is fixed by balancing the derivative and ramp terms against the nonlinear saturation term. It therefore depends on `n`.

The two exponents must not be conflated.

# Cubic Specialization

For the cubic case:

`n = 3`

the generalized dynamics become:

`dC/dt = v_eff t C − gC³`

The rescaling is:

`t = v_eff^(−1/2) τ`

`C = g^(−1/2) v_eff^(1/4) y`

and the reduced equation is:

`dy/dτ = τy − y³`

Therefore:

`t_delay ~ v_eff^(−1/2)`

`C_critical ~ g^(−1/2) v_eff^(1/4)`

For the normalized coefficient `g = 1`:

`C_critical ~ v_eff^(1/4)`

The cubic saturation order changes the amplitude exponent to `1/4`; the temporal exponent remains `−1/2`.

# Geometric Closure

A geometric closure may be introduced when the reduced coherence amplitude is associated with a full-dimensional coherent measure.

For a `d`-dimensional coherent structure:

`V_coh,d ∝ C_1 C_2 ... C_d`

Under an isotropic reduction:

`C_1 ~ C_2 ~ ... ~ C_d ~ C`

this becomes:

`V_coh,d ∝ C^d`

A model may then adopt the dimensional closure:

`n = d`

For `d = 3`:

`V_coh,3 ∝ C_x C_y C_z ∝ C³`

and the selected saturation order is:

`n = 3`

This is a model closure connecting a volumetric coherent measure to the order of the leading saturation term. Spatial dimensionality alone does not constitute an algebraic proof that every three-dimensional system must have the normal form `−gC³`.

# Symmetry Closure

A separate closure follows when `C` is a signed amplitude and the reduced dynamics are invariant under:

`C → −C`

Under this symmetry, the vector field must be odd in `C`. Even powers are excluded from the leading symmetric normal form.

The first nonlinear odd power above the linear term is:

`C³`

The leading symmetric saturation term is therefore:

`−gC³`

This argument is independent of the geometric closure. It follows from sign symmetry of the reduced amplitude, not from spatial dimensionality.

# Three-Dimensional EDC Specialization

In the three-dimensional EDC specialization, two independent model arguments may support the cubic term:

1. geometric closure: `V_coh,3 ∝ C_x C_y C_z`, with isotropic reduction `V_coh,3 ∝ C³` and selected order `n = 3`;
2. symmetry closure: the transformation `C → −C` excludes even powers and leaves the cubic term as the leading nonlinear saturation.

When both assumptions hold, they support the same cubic normal form:

`dC/dt = v_eff t C − gC³`

They remain logically distinct and must be documented separately.

Neither closure changes the temporal result:

`t_delay ~ v_eff^(−1/2)`

# Relation to Endogenous Drift Variables

When the effective ramp velocity is represented locally as:

`v_eff = μP`

with `μ > 0` and positive local destabilizing pressure `P`, the temporal law becomes:

`t_delay ~ (μP)^(−1/2)`

For the cubic specialization, the amplitude law becomes:

`C_critical ~ g^(−1/2)(μP)^(1/4)`

This substitution does not alter the exponent balance; it only expresses `v_eff` through the local drift parametrization.

# Scope and Boundary of Application

The lemma applies when:

- the local critical ramp is linear in time and enters as `v_eff t C`;
- `v_eff > 0`;
- `g > 0`;
- `n > 1`;
- `gC^n` is the leading saturation term in the analyzed local regime;
- `C^n` is defined on the analyzed amplitude domain;
- the reduction to a single critical amplitude is valid over the interval being analyzed.

The exponent balance must be re-derived when:

- the ramp is nonlinear in time;
- the control parameter enters through a different power of `C`;
- several nonlinear terms remain co-leading;
- memory, delay, nonlocality, multiplicative noise, or additional critical modes alter the dominant balance;
- the single-amplitude reduction is not valid.

The lemma is an algebraic scaling result for the stated normal-form class. Geometric and symmetry closures select a model specialization; they are not part of the exponent-balance proof itself.

# Repository Integration Rule

Within this repository:

- `−1/2` is the temporal exponent for the stated linear-ramp class;
- `1/(2(n−1))` is the `v_eff` amplitude exponent;
- `−1/(n−1)` is the `g` amplitude exponent;
- the cubic model uses `n = 3` and therefore amplitude exponent `1/4`;
- geometric and symmetry closures are stated separately;
- no temporal exponent is inferred directly from spatial dimensionality or from the saturation order alone.

Related specialized derivations:

- [Canonical Critical Form and Scaling Law](canonical_critical_form_and_scaling_law.md)
- [Scaling and Criticality](scaling_and_criticality.md)
