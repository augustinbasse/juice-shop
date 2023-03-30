# MaquetteDSO

# This code repository groups all the latest.gitlab-ci.yml templates that can be used to create security pipelines.

# Before importing these templates you should set up the following variables
They can be set up through the GitLab interface, in Settings > CI/CD > Variables > Add variable <br />
The variables are written bellow as KEY : Value <br />
For exporting scan reports to Defectdojo: 
<ul>
<li>DEFECTDOJO_PRODUCTID : The product ID of the targeted product in DefectDojo (ex: 6) </li>
<li>DEFECTDOJO_TOKEN : The api token / api key of the DefectDojo instance used (ex : 548afd6fab3bea9794a41b31da0e9404f733e222) </li>
<li>DEFECTDOJO_URL : The base url followed by /api/v2 of the DefectDojo instance used (ex : https://demo.defectdojo.org/api/v2) </li>
</ul>
To integrate snyk scans in your pipeline: <br />
<ul>
<li>SNYK_TOKEN : Your user token that can be found on the snyk interface in your account (bottom left) > Account settings > Auth token</li>
</ul>
To use the docker-deploy script: <br />
<ul>
<li>PROD_BRANCH : The name of your production branch. Only merge requests to this branch will trigger the docker-deploy.yml script</li>
</ul>



# The use of the different templates is described here

gitlab-defectdojo.yml : used to link defectdojo to gitlab, whenever the pipelines run, create an engagement inside a defectdojo project and import the specified scan results (done with other complementary templates). <br />
Choose witch scan results to import by selecting in the following templates: <br />
   TODO
    
