# software-foundations

Answers to the [Software Foundations][] course book by Benjamin C. Pierce et al.

## Progress

- [x] Preface
- [x] Basics
- [x] Induction
- [x] Lists
- [x] Poly
- [x] MoreCoq
- [x] Logic
- [ ] Rel
- [ ] Prop
- [ ] MoreLogic
- [ ] ProofObjects
- [ ] MoreInd
- [ ] SfLib
- [ ] Imp
- [ ] ImpParser
- [ ] ImpCEvalFun
- [ ] Extraction
- [ ] Equiv
- [ ] Hoare1
- [ ] Hoare2
- [ ] HoareAsLogic
- [ ] Smallstep
- [ ] Auto
- [ ] Types
- [ ] Stlc
- [ ] StlcProp
- [ ] MoreStlc
- [ ] Sub
- [ ] Typechecking
- [ ] Records
- [ ] References
- [ ] RecordSub
- [ ] Norm
- [ ] LibTactics
- [ ] UseTactics
- [ ] UseAuto
- [ ] PE
- [ ] Postscript

## Tactics quick reference

Here are the most commonly used tactics.

- `intros`:
  Move hypotheses/variables from goal to context

- `reflexivity`:
  Finish the proof (when the goal looks like `e = e`)

- `apply`:
  Prove goal using a hypothesis, lemma, or constructor

- `apply... in H`:
  Apply a hypothesis, lemma, or constructor to a hypothesis in
  the context (forward reasoning)

- `apply... with...`:
  Explicitly specify values for variables that cannot be
  determined by pattern matching

- `simpl`:
  Simplify computations in the goal

- `simpl in H`:
  ... or a hypothesis

- `rewrite`:
  Use an equality hypothesis (or lemma) to rewrite the goal

- `rewrite ... in H`:
  ... or a hypothesis

- `symmetry`:
  Changes a goal of the form `t=u` into `u=t`

- `symmetry in H`:
  Changes a hypothesis of the form `t=u` into `u=t`

- `unfold`:
  Replace a defined constant by its right-hand side in the goal

- `unfold... in H`:
  ... or a hypothesis

- `destruct... as...`:
  Case analysis on values of inductively defined types

- `destruct... eqn:...`:
  Specify the name of an equation to be added to the context,
  recording the result of the case analysis

- `induction... as...`:
  Induction on values of inductively defined types

- `inversion`:
  Reason by injectivity and distinctness of constructors

- `assert (e) as H`:
  Introduce a "local lemma" `e` and call it `H`

- `generalize dependent x`:
  Move the variable `x` (and anything else that depends on it)
  from the context back to an explicit hypothesis in the goal
  formula

## License

See [LICENSE][].

[Software Foundations]: http://www.cis.upenn.edu/~bcpierce/sf/current/
[LICENSE]: ./LICENSE
