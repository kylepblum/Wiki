## VAE 
:Lee: :Aldo: :Raeed: :Yufei:  

### Motivation
- We want to feed muscle receptor inputs into a VAE to reproduce cortical proprioceptive mappings
### Actions
- [X] Review Yufei's code
- [X] Get Raeed's monkey data
- [ ] Try to run spindle model through muscle lengths
- [ ] Train model on muscle lengths, optimize on muscle lengths
- [ ] Train model on muscle lengths, optimize on muscle velocities
- [ ] Train model on spindle inputs, optimize on muscle lengths/velocities
- [ ] Train model on each inputs set, optimize on S1 (3a?) firing rates

### Notes
[Simulation workflow](VAE_workflow.md) 



### Misc
- Questions for Yufei
  - What properties does the input data need to have? I'm importing it, and the model returns NaNs
  - What is this K parameter ("numbers of samples each time")
  - How many iterations does this really need?
  - How much data does it need? It returns NaNs when there's a lot of data
  - 

