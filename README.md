# Lord


Objective : To develop an AI model that help SMBs find verified solutions to simplify the sourcing, evaluation, and selection of telecom, mobility, and IT services and solutions.
Implementation : The complete model architecture and training process is based on federated learning and semi supervised mode of training each client model this helps to capture new variants of data also.
Applications : The model trained has wide range of applications and is applicable to new releases and new variants of data as well. It can be used by all SMBs to select most suitable service, products and application for there purpose.
Problem Statement:
IT products and services are evolving constantly at a high pace. High complexity in selecting suitable products for business use case. SMBs ( Small Mid-Sized Business often lack human resource to cope up with selection complexity.
     1)How do SMBs more easily and efficiently sort out the thousands of options available to them?
      2)How to build tools that help SMBs find verified solutions to simplify the sourcing, evaluation, and selection of telecom, mobility, and IT services and solutions.
Moving towards industry 4.0 leads to booming increase in IT services build Finding a service for particular business is like finding a pin in sand heap.
SMBs find it really challenging and time consuming to select a service best suited for them. Data leaks due to centralized database storage.
Lack of AI powered solutions.
Loopholes in Current Techniques:
Human Intervention in selection best suitable technologies. Lack of staff and heavily time consuming in selecting best services for SMBs. Unverified usage leads to loss in business if efficiency is up to the mark, Utilization of higher efficiency products that required leads to loss in business. Booming services leads to many fake products and SMBs become victims.
Dataset Creation
Dataset in Real Life 
Large organizations or any business who is releasing or have used a particular software can give rating for some features ( 10 features in our case ) on any portal of their business.
These portals act as clients in Federated Environment
Since this data is private they are resistant to sharing it.
Here is when Federated Learning comes as savior and helps in training a global model based on all such federated datasets around the globe with high data security as no data is seen while training.
Global Model is trained using several client end points to predict few features (4 features in our case) to get overall idea of the service being offered.
Using this global model as backend any SMBs can get idea of which product or IT service they should opt for based on their requirements.
How Framework works:
User Sign up / login on the portal. A screen with three options is shown. Recommend Products Based On desired features. Check information and efficiency of any product by its ID/Name. Check products with similar scores. Check products with similar predicted features. In each of the three inputs. A set of required response is displayed via API calls. In first case global model predicts and recommends based on the predictions In second case scores of the products are used for find similar products In third case the 4 output features are used to match required recommendations of the services
Advantage of Proposed Solution
Consistency – Training and fetching data in decentralized (federated) way helps to maintain consistency throughout the process. Fault Tolerance – Federated Learning based training is fault tolerant as failure of any client does Communication – Communication Cost is very low using Federated Modelling as compared to Centralized Learning. Security – Security of data is maintained as no data is being accessed on clients end during training. Decision making time - SMBs are able to make quicker decisions based on one step login and based on requirements they receive recommendations in no time.
Business Points
Human Intervention is not required from SMBs end. Quicker decision making process. SMBs are able to work and cost cutting is there by getting recommendations on there best needs. SMBs can work on new tech and spend more time on developing the idea rather than thinking about the products and services. The recommendation system can be used as a SaaS service itself to a wide range of people ranging from individuals to MNCs. System is very much secured hence building trust is easily facilitated.

