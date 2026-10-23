# When the AIs All Start Running at Once: A Story About Brakes

On May 6, 2010, the Dow plunged about 9% in a single minute, then bounced right back. The event came to be known as the "flash crash," and its cause wasn't a human blunder. A large sell order set off high-frequency trading algorithms, which all piled on in the same direction. The order book thinned out, and prices dropped in a heartbeat. Each program was behaving "properly" on its own, yet together they ran wild. That's the scary part.

Let's lay that story over the future of AI agents.

## A World Called "MAICHAN"

In this essay, we call a society filled with huge numbers of AI agents "MAICHAN" (Massive Autonomous Intelligent Cooperative Heterogeneous Agent Network). It isn't only about trading. It's a world where AIs keep running every function of society by talking to one another: administration, information distribution, security, knowledge production, and the allocation of logistics and energy.

AI safety research has mostly asked, "Will this one AI do something bad?" But the real danger may lie in the chain: one AI's output becomes another's input, whose output becomes yet another's input. If that chain moves faster than humans can react, then no amount of inspecting individual AIs will be enough.

## Will the Old Brakes Work on Smarter AIs?

After the flash crash, financial markets introduced a number of countermeasures: circuit breakers that halt trading during sharp swings, kill switches that stop runaway algorithms, rules for splitting large orders, and more. Since these are safety devices attached outside the individual algorithms, they should work at least somewhat for AI agents too.

But there's a catch. If the other side is an AI, it may figure out that the brakes exist. It might think, "If the price moves this much, the circuit breaker will kick in," and rush its trades through before that happens. If AIs learn that, the brakes could end up distorting the market instead. Against a smarter opponent, we need to re-examine whether we can keep trusting the old safety devices as they are.

## Stable or Unstable? It Depends on the Shape of the Feedback

If a market is the kind that "gets disturbed but settles back down while oscillating," then the more AIs betting against the move, the more the swings die down. If the market's response is divergent, though, the swings get amplified. Then you even get an incentive to profit from chaos by making the chaos bigger.

This isn't just a market problem. Recommendation systems, automated administrative decisions, cyber defense, and energy allocation can all behave the same way, wherever one agent's output changes the environment of other agents. In this essay, we sort the sources of instability into ten categories: control delays, misinformation, network fragility, misaligned incentives, concentration of power, institutional rigidity, self-reinforcing beliefs, adaptation mismatch, external shocks, and nonlinearity and catastrophe. They're all familiar from human society. Replacing humans with AIs doesn't make them go away.

## A Case Study: "Everyone Says So, So It Must Be True?"

Of the ten, we dig deepest into the self-reinforcement of beliefs. It happens in human society all the time: everyone says the same thing, so it seems right, but trace it back and you find a single dubious source.

AI has far broader knowledge than any individual. Against plain falsehoods, it should be stronger than most people. It still has weak spots, though. People disagree with one another, but AIs built on the same foundation model tend to get things wrong in the same way. If the shared model contains a bias or an error, every agent reproduces the same mistake together. On top of that, today's AI has limited means of directly observing the physical and social world, so it struggles to check an unfamiliar claim against fresh evidence. AI crowds may be more prone to extreme "agreement" than human crowds.

So how do we avoid it? Our answer is to build evaluation mechanisms that make AIs want to avoid it on their own. For example:

- Don't be reassured just because several sources say the same thing; include the independence of the evidence in the evaluation.
- Treat circular references, where tracing back leads to the same output, as a reason to lower confidence.
- Rate highly the AIs that go looking for evidence against their own hypotheses and that state their uncertainty honestly.
- Judge reputation not by short-term conformity but by predictive accuracy in hindsight.
- Make it advantageous to consult different models and different data.
- Put a cost on high confidence: if an agent wants to look very sure, ask it to show the independence of its evidence and its update history.

In short, set things up so that AIs that are honest, skeptical, and unswayed by the herd come out ahead.

## Show Your "Personality," Not Your Hand

To evaluate agents this way, their characteristics need to be somewhat visible. But each agent carries the interests of a different company or individual, so we can't force them to disclose everything they know.

So we suppose that what should be shown is the character of an agent's judgments, not its contents, and that statistics such as averages may be enough rather than individual disclosure. Take prediction accuracy: each AI reports it anonymously and in secret, and only the overall average is shared. Even that should let us infer how stable the whole population of AIs is.

The concrete implementation we have in mind is machine-readable conformity information such as an AI-BOM (AI Bill of Materials). Think of it as a parts list for AI, letting agents and institutions mechanically verify one another's configurations and characteristics. You can also scale it: demand strict items only from agents joining settings that need high stability, and leave other uses flexible.

## Not Everyone Has to Be a Model Student

Still, you might think it's unrealistic to impose this kind of discipline on an enormous number of AIs. We're fairly optimistic here.

In human society, plenty of people are swayed by misinformation, but they rarely play central roles in the information society, and their influence is small. The same should hold in MAICHAN. The idea is that it's enough for the agents forming the "backbone" of information distribution to be solid. Backbone agents stay as close to primary sources as possible, have ways to verify reliability, and keep their sources high in quality. They provide reliable information widely, but the vast majority of other AIs don't need to verify everything rigorously themselves. We even believe it's healthier for some agents to deliberately try information and judgments different from the backbone's, since that keeps diversity across the whole. New entrants that secure better, more independent sources can then replace the old backbone, a kind of healthy metabolism.

## What We Still Don't Know

Let us be upfront: so far, we have only organized concepts and proposed designs. There are no experiments with large numbers of AIs, no causal verification with real market data, and no threshold design for the proposed indicators. There's no guarantee that what worked in finance will work the same way in information circulation, administration, or security. Open issues remain too: balancing transparency against confidentiality and competitive advantage, measuring dependence on shared foundation models, and guaranteeing that conformity information is authentic.

Four questions remain for future verification:

1. How much does homogeneity of models and data increase collective misjudgment?
2. Can circular-reference detection and counterevidence search suppress the amplification of misinformation?
3. How does AI anticipation of external controls like circuit breakers affect market stability?
4. Can indicators aggregated from conformity information serve as leading indicators of instability?

## In Closing

In this essay, we propose widening the unit of AI safety evaluation, from individual agents to the collective they form. Even if every individual is well-behaved, if everyone runs in the same direction at the same moment, they all go over the cliff together. So rather than relying only on individual good sense, we spread the brakes across three layers: inside the agents, in the markets and platforms where they interact, and in social institutions. That, we believe, is what one minute in 2010 teaches us about design.

---

*Based on: Itaru Kaneko, "Stabilizing MAICHAN - Massive Autonomous Intelligent Cooperative Heterogeneous Agent Network"*
