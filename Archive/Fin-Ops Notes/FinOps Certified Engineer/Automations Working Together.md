## Integration

Automation tools rarely operate in isolation. Integration between tools can be very powerful, and something you may want to take advantage of. You'll want to avoid having many separate tools that do their own version of the same thing. For example, if you have an existing ticketing system at your organization, you would ideally implement FinOps tooling that will generate tickets for action items in that existing system instead of building in a separate task-tracking system.

## Automation Conflict

As you implement more types of automation and different tools of automation, you increase the likelihood that one automation impacts another. 

For example, Automation A is an auto-scale group trying to scale up groups and Automation B is tag enforcement that sees these new things are not properly tagged and deletes them. To avoid automation conflict, ideally, the automations are aware of each other and one is understood to be the primary decider. However, this is not always realistic. More likely, to avoid conflict, automations will be contained into defined boundaries. This might mean that you have Automation B (tagging compliance controls) in the pre-production environment but not in the production environment. This way conflict will be contained to the pre-product environment.  

Automation conflict is another factor to consider when building or buying automations. This can increase the time it takes to integrate automations together and watch for conflicts. 

### **Lessons Learned the Hard Way**

Joe Daly, formerly Director of Cloud Optimization at Cardinal Health and Nationwide, tells the story of how he accidentally took down a production environment by manually removing a nonproduction resource tied via automation to the production one. A stated earlier, education about automation being used is critical in the organization. To hear the full story, check out [Episode 13(opens in a new tab)](https://open.spotify.com/episode/1kOyio4WOwii2bM6wFRjUy?go=1&sp_cid=b149981b5b05fea7cb08f475fad8ba37&utm_source=embed_player_p&utm_medium=desktop&nd=1) of the FinOpsPod podcast. 

## Safety & Security

Often, FinOps automation requires very high levels of access to your cloud environments, whether it’s just the ability [for an automation to have environment permissions] to describe how everything in your account has been configured, or the ability to change (start/stop/delete) the resources themselves. Such access could lead directly to a denial of service attack, data loss, corruption, or a confidentiality breach. Security is often cited as a major reason third-party tooling isn’t used inside organizations. It’s understandably difficult to get a security team to sign off on the use of a third-party tool that needs broad access to cloud accounts.

Remember, safety and security is a drawback of automation. You can partner with your FinOps practitioner to assess options for automation and dive deeper into safety and security concerns.

#FinOps 