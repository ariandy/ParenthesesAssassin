<a href="">
  <img src="https://img.shields.io/badge/Version-0.0.2-blue.svg"/>
</a>
<a href="">
  <img src="https://img.shields.io/badge/Written_By-Ariandy-green"/>
</a>

# λ-PRcSA
```
!!! Before you read this stuff, make sure you got the first principle of Lambda Calculus. !!! 
```
In my sophomore year, I shoot myself in the foot by learning about pure functional programming theory autodidactly. But first thing first, you must make the good grasp about the fundamental on this topic, (and here we are) Lambda Calculus.

Solving the Lambda Calculus is quite fun for sure. Like a puzzle, you played it with certain rules.
Even though this is just small baby steps, but sometimes, it's intimidating enough if the form of expression written in lengthy one-liner, and absolutely, nested parentheses.

Let's see some examples:

```
((((λf.(λg.(λx.((fx)(g x)))))(λa.(λn.(n a))))(λn.z))p)
```
```
((λf.((λg.((f f)g))(λq.(k q))))(λx.(λy.y)))
```
See? It's pretty complicated.
```
Um, hey. Ariandy, I already solved it painlessly.
```
Ya, I know, I know. Any of us know how to reduce it smoothly and transform it into `β-normal form`.
But, vice versa, the other people out there got the bottlenecks from those expressions, feel unmotivated and discouraged in the end of the day.

**This is my own hypothesis. I think, it's one of many reason why functional paradigm still not the norm.** <br>
Ya. It's a bare minimal concept you must have under your belt if you wanna learn about pure functional programming.
But ironically, so many people give up after got this bottlenecks.

So, back in the day (2014), I made a pedagogical way to solve those lengthy-nested-form.<br>
And I named this method as **Smashing-In-Detail**.<br>
I named it after my favourite war tactics / campaign strategy in The Battle of Shenandoah, **Defeat-In-Detail**, doctrinal military terms that means **to defeat an enemy by destroying small portion of its armies instead of engaging its entire strength**.

## Tactics
Let me repeat the explanation about Defeat-In-Detail.
```
... to defeat an enemy by destroying small portion of its armies instead of engaging its entire strength
```
We use the same idea to eliminate the parentheses ambusher.
```
Wait a sec, Ri. Is it a different set of rules to eliminate those things?
```
Absolutely, **NO**. Still stick to the Lambda Calculus rules (`α-equivalence`, `β-reduction`, currying, etc)!<br>
It's just an additional way to carefully reduce all of 'em (except the divergence one).

So, this is the plan:
- **λ** (Still stick to Lambda Calculus doctrine)
- **P**eeling off layered parentheses
- **R**emove outer/useless/redundant parentheses
- **c**lean the leftmost/outermost Lambda from parentheses
- **S**eparate (Divide & Conquer) the one-liner expression, if possible
- **A**ssault the separated expressions

Because this stratagems, sometimes I call it **λ-PRcSA**.

## Coming soon
- I wanna elaborate the rules of λ-PRcSA.
Once again, I don't explain the basic of Lambda Calculus on this stuff. If you read this, I expect you already grasping the basic rules of Lambda Calculus and know how to evaluate the shorter expressions.
