# To Change BCs:
(1) In search.py, before line 196, add:
def New_BC (ind,result):
  #how to get the BC
  #for static BC (like how many coins on the map) of a level, get it from im=np.array(json.loads(ind.level))
  #for dynamic BC (like how many coins the AI acutally collects), get it using the "result" parameter, which is a game result
  #return a value
 
(2) In config/cma_me.tml, change the featureX and featureY to the exactly the name of the function ("New_BC" in this case)
 
 

# To Train GAN:
src/GANTraining/main.py

# To Run CMA-ES/CMA-ME/MAP-ELITE on trained GAN:
search.py
