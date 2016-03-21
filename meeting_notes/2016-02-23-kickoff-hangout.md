#Ops NTSB Meeting Notes
##2016-02-23
_[Marc note: I may have mis-transcribed some of this, all errors are mine, please feel free to correct.]_

__Participants:__

* Ben Krueger, Slalom Consulting (benjamin@xxxxx)
* Charity Majors, Hound (charity@xxxxx)
* Marc Hedlund, Fiasco, Inc. (marc@xxxxx)
* Aaron (from Kickstarter)
* Sam
* Jonathan Gilbert (jong@xxxxx)
* Tim McGinnis (st.lart@xxxxx)

__Intro chat; purpose__

Ben: Desire to have some shared communication about learning from failure. Shared industry knowledge about past failures is poor. (Charity mentions [SRE Weekly](http://sreweekly.com/).) Would be useful if we started with (1) a standard format, and (2) a repository for them.

Charity: are we talking about people sharing the postmortems they’re already making, or doing something new, like having an investigatory board that would get people to try new things? Are we talking about social and legal problems in a bigger way? (Do you need legal force to make this work at all?)

Ben: on the other hand, if we don’t start sharing info voluntarily, it’s likely regulation will be imposed as failures become bigger or have great impact (e.g. CA security breach laws). Things we’re doing are impacting peoples’ lives in a bigger way.

Charity: (1) non-profits are legally required to disclose this sort of information already. (2) small companies might be more willing to participate since they have less to lose and could build credibility with a “badge of honor/respect” because they’re participating.

__Benefits of a shared group__

Sam: after some recent outages we’ve had a lot of discussions about how to be public about some things, so that technical users can gain confidence in the reaction, but the greater industry doesn’t provide a lot of good models or guidelines. People across a group of companies could be really useful, helping to have higher confidence (e.g. Google management practice or the like). I think we would get behind almost an open standard for this sort of review and understanding. Debate about whether we were pursuing the right kind of communication.

Charity: So here are questions to ask yourself, how to ask them, starter or feeder questions, ways to make postmortems productive. List of things you should leave any postmortem with.

Sam: Useful to have persuasion around blamelessness, we could have roundtables, a lot of contribution we could make.

Charity: I love the idea of a person with fresh eyes, no background on the company but understanding of the technical issues, to get fresh perspective on the events.

__Incentivizing companies to participate__

Ben: Would it help to have PR resources to help develop a message for companies that decide to participate? How could we make companies more comfortable with this? Would companies fear engineers publishing secrets and judgments, and would having experienced PR people make more companies comfortable?

Charity: Nothing should be published by the committee that hasn’t been anonymized! It would be way better if we could do it in a non-identifiable way. Yearly report?

Ben: [Data Breach Report from Verizon](http://www.verizonenterprise.com/DBIR/2015/) might be a good model.

Marc: Would we lose value by anonymizing and losing important details?

Charity: Yeah, maybe right, and we should be de-stigmatizing this, not hiding it necessarily.

Ben: We do have companies that are doing this already but not in a standard way.

Charity: If Github is in, I’m in… (common reaction, perhaps?)

Ben: Netflix, Github, Amazon, once they do something, other companies might be interested.

Charity: Excellent public postmortems are also good for recruiting, and a good sign.

__Anonymization and concrete outputs__

Aaron: I’m on the ops team at Kickstarter. One thing I’m struck by is the parallels to the security community, there are groups that do this but there are very informal, confidential networks (you have to know the right person to get in). The benefit is that leads to a safe space and leads to more comfort. The big downside is that it’s all pretty closed, unless you know the right person to ask. Maybe this is a strong pattern to start to get people to be more comfortable?

Ben: I can see that but what would the output of that be? I think the general goal should be to generate artifacts that people can learn from; if we use FrieNDA as a model, does that give us enough of the benefit for those outside of the inner circle?

Aaron:  Sure, agree, but that’s a community that has already addressed this problem in one way, albeit a closed way. One thing to keep as a concern is that the time invested to make a postmortem that could be shared with the world would be a huge amount (versus the investment for internal sharing), and we would need to have tools or practices (std formats or whatever) to reduce that investment if we expect this to be frequent.

Ben: Agree, blueprints/templates or examples would be very helpful. There’s probably a bar, too, where an incident is not significant enough to be shared with the community.

Charity: We’re looking for complex, cascading failures — we don’t usually have outages that are caused by some one thing, but instead when things go wrong in chains or webs.

Marc: Agree, but sometimes a single remediation might be worthwhile even if the failure was minor (example of nighttime indicators in the Etsy deploy tool as a reminder that people are deploying after hours). Maybe “Pattern Language” style successful remediations would work.

Ben: Some good thresholds, maybe, similar to “plane fell out of sky” or “person died” for NTSB [Marc note: I may have mis-transcribed this.]

Sam: Maybe a study of things that work at different companies would be useful — central knowledgebase from the real world.

Jonathan: How does this work? Do you have to contribute to learn from it?

Ben: I’d love for the output to be for the general community, not closed.

Marc: [Example of the Engineering Exchange Program](https://codeascraft.com/2012/09/10/the-engineer-exchange-program/). Even though the first one was not successful on both sides, it was perceived as successful and increased the confidence of other companies, where there was more success.

__So how can we get this going?__

Ben: So how can we get the ball rolling? Big example, signup, etc? Disagree that this is an impossible task, but we should be realistic about the things to overcome.

Charity: Could we get going with a tool that we’re generating ourselves and get things going with examples, and then build from there, ramp up the public participation over time?

Ben: Github repo of past examples would be great.

Charity: Would love to do “book reports” about existing postmortems and what we’ve learned from them.

Marc: Great idea, [Dan Luu’s examples](http://danluu.com/postmortem-lessons/) (see also [Github repo](https://github.com/danluu/post-mortems) ) are awesome.

Jonathan: Yeah, if there were more that we would get from postmortems, we might have more attention to them and get more out of them.

Ben: Will start Github repo, we should work towards a postmortem format. Charity, willing to write the first book report?

Charity: Totally, on it. Also, we should make a statement about this. What’s the idealistic paragraph about what we’re trying to do with this?

Ben: Reading NTSB and other examples are super useful.

Jonathan: Also useful to have eye on customer impact.

Ben: One final thing: maybe offer a review service to a company that chooses to publish one — maybe help companies make sure they’re doing a good job of it before publishing. That could be a good first step, especially if the offered investigation turns out to be useful to the company.

Sam:  I agree with Charity’s comment about a mission statement. Also, it would be good to ask customers about what they’d want to know about from postmortems. That might give us ideas about things we can deliver. Really high-quality examples of writing and forms of discussion would be extremely useful to the community.

ACTIONS:

- [x] Mission statement - Charity (in for a rough draft, welcome collaboration)

- [ ] Examples of great and worthwhile existing public postmortems- OWNER NEEDED

- [ ] A few book reports about existing public postmortems - Charity for the first one

- [ ] Talking to customers/consumers of postmortems about what they might want to see in them- OWNER NEEDED

- [ ] Recruiting companies to get involved - OWNER NEEDED

- [ ] Develop an open sourced post-mortem report format - OWNER NEEDED

- [ ] Find a way to solicit and accept feedback from companies and individuals about: what they would like to know about when learning from an incident. - OWNER NEEDED

- [X] Create a GitHub repo to store artifacts we generate - Ben

- [ ] Should write a blog post about some of these ideas. Goes towards recruiting other companies to participate. Depends on mission statement. - Ben

