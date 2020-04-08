cd to /echosvc folder 


docker build -t anushree-echomain .
docker tag anushree-echomain anuacrteam1.azurecr.io/anushree-echomain:v1
docker push anuacrteam1.azurecr.io/anushree-echomain:v1
