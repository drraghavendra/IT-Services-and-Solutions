#IT SERVICES AND SOLUTIONS


Objective : To develop an AI model that help SMBs find verified solutions to simplify the sourcing, evaluation, and selection of IT services and solutions.

Implementation : The complete model architecture and training process is based on federated learning and semi supervised mode of training each client model this helps to capture new variants of data also.

Applications : The model trained has wide range of applications and is applicable to new releases and new variants of data as well. It can be used by all SMBs to select most suitable service, products and application for there purpose.

Problem Statement:
IT products and services are evolving constantly at a high pace. High complexity in selecting suitable products for business use case. SMBs ( Small Mid-Sized Business often lack human resource to cope up with selection complexity.
     1)How do SMBs more easily and efficiently sort out the thousands of options available to them?  2)How to build tools that help SMBs find verified solutions to simplify the sourcing, evaluation, and selection of  IT services and solutions.
Moving towards industry 4.0 leads to booming increase in IT services build Finding a service for particular business is like finding a pin in sand heap.
SMBs find it really challenging and time consuming to select a service best suited for them. Data leaks due to centralized database storage.
Lack of AI powered solutions.
Loopholes in Current Techniques:

Human Intervention in selection best suitable technologies. Lack of staff and heavily time consuming in selecting best services for SMBs. Unverified usage leads to loss in business if efficiency is up to the mark, Utilization of higher efficiency products that required leads to loss in business. Booming services leads to many fake products and SMBs become victims.
Dataset Creation
Dataset in Real Life 
Large organizations or any business who is releasing or have used a particular software can give rating for some features ( 10 features in our case ) on any portal of their business.These portals act as clients in Federated Environment.Since this data is private they are resistant to sharing it.
Here is when Federated Learning comes as savior and helps in training a global model based on all such federated datasets around the globe with high data security as no data is seen while training.Global Model is trained using several client end points to predict few features (4 features in our case) to get overall idea of the service being offered.Using this global model as backend any SMBs can get idea of which product or IT service they should opt for based on their requirements.

How Framework works:

User Sign up / login on the portal. A screen with three options is shown. Recommend Products Based On desired features. Check information and efficiency of any product by its ID/Name. Check products with similar scores. Check products with similar predicted features. In each of the three inputs. A set of required response is displayed via API calls. In first case global model predicts and recommends based on the predictions In second case scores of the products are used for find similar products In third case the 4 output features are used to match required recommendations of the services.

Advantage of Proposed Solution
Consistency – Training and fetching data in decentralized (federated) way helps to maintain consistency throughout the process. Fault Tolerance – Federated Learning based training is fault tolerant as failure of any client does Communication – Communication Cost is very low using Federated Modelling as compared to Centralized Learning. Security – Security of data is maintained as no data is being accessed on clients end during training. Decision making time - SMBs are able to make quicker decisions based on one step login and based on requirements they receive recommendations in no time.

Business Stand Point

Human Intervention is not required from SMBs end. Quicker decision making process. SMBs are able to work and cost cutting is there by getting recommendations on there best needs. SMBs can work on new tech and spend more time on developing the idea rather than thinking about the products and services. The recommendation system can be used as a SaaS service itself to a wide range of people ranging from individuals to MNCs. System is very much secured hence building trust is easily facilitated.

====Requirements====
Python
NodeJS
JavaScript

====File Structure====

  -APIS (Having APIs for user LogIn/ SignUp Data)
    -env (Python Environment)
    -credentials ( Static Database for Credentials for Demo ) 
       credentils file
    - main ( Main File having APIs for LogIn, Sign Up)
  
  -FL Models ( Files to train the model using Federated Learning )
    -CreateDataset.ipynb ( To create the generic real world dataset)
    -FederatedLearning.ipynb ( To train the model using FL )
    -mnistAlpha_FL_0_1.ipynb ( To Analyse the Pseudolabeling Semi Supervised Classification Result)
    -restApiProduct.ipynb   ( To create Endpoints for Service/Product Recommendation System)
  -public (To store the trained models)
     -models (Trained models)

  -server (GraphQL Server for SignUp /LogIn)
     -src
       -datasources (Datasources Components for APIs)
       --graphql (Resolvers and schemas for APIS)

  src ( Front End using React and Node JS)
   -apis ( APIs for Product Recommendation System )
     -main.ipynb
  -assests (Common Image files used )
     - many image files
  -components ( Components for the UI)
     -Efficiency
     -EfficiencyResult
     -Footer
     -Recomendation
     -SimilarFeature
     -SimilarProduct
     -SimilarRating
   -dataset ( Dataset for the Produts/ Services)
     -dataset.csv
     -dataset.json
   -pages (UI Pages)
     - pages for different screens
   -services (Service)
     -ProductService


====File Description====

==Backend (Python) ===
CreateDataset.ipynb: This notebook creates a synthetic dataset which we have used in our backend and training of the machine learning model under Federated Settings

FederatedLearning.ipynb: This notebook explains the Exploratory Data Analysis and overall training of the global model with client models under Federated Settings. Four models each for Security, Scalability, Ease Of Use, Latency are trained under Federated Settings.

mnistAlpha_0.1_FL.ipynb: This notebook is an example of how pseudo labellings can be used in our problem statement to introduce semi-supervised learning with only 10% labelled data.

==Frontend (React code base) ===

Please follow these commands to create react project and install required nodejs dependencies.
npx create-react-app fl-aotmp            =>  Create the project

npm install bootstrap --save             =>  Install Bootstrap

npm intall react-router-dom              =>  For Router, Switch

< Install Other required Dependencies >

npm start

restApiProduct.ipynb                  =>     Host api end points as server using colab


=> Copy Generated Public URL and enter in  PRODUCT_API_BASE_URL  in services/ProductsService.js  file.  Eg : const PRODUCT_API_BASE_URL = "http://9d78-34-86-177-191.ngrok.io";
