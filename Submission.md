1. Launch EC2 instance--> Ubuntu Server 22.04 LTS--> t2.medium--> Storage: 20 GiB gp2 ![1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/aed4d66c-037c-40c7-be7f-ad6fa1c61113)


2. Login with ssh--> sudo apt update--> sudo apt install npm -y--> sudo apt upgrade nodejs--> node -v  ![2](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/aa35ca70-ebeb-4a15-b725-6f7b177c2504)
![2 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/c914abc6-b20d-4451-9fbe-bb73e4d85c36)


3. nano Dockerfile--> cat Dockerfile ![3](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/3058a90d-f5b0-4724-873d-106091ad0361)


4. nano buildspec.yml--> cat buildspec.yml ![4](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/cfbd2ba2-52d4-4a0f-85dc-de66b5da7b1f)


5. sudo apt install docker.io -y --> sudo usermod -aG docker $USER--> exit--> re-login ![5](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/ce1901b8-0da3-4fd0-8932-2186da8f93fe)
![5 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/c6e60ce7-8001-4a33-b1c8-172c0e55f267)


6. sudo apt install git -y ![6](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/cb73aafd-8e4a-433c-89e7-fe375583d553)


7. sudo apt install awscli -y ![7](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/76438807-4abb-44c0-8036-e92c54b6cfa5)


8. aws configure ![8](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/33a66538-2ba1-4aca-b19e-a4c7985e6a93)


9. npx create-react-app weekly-task-app ![9](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/0035d482-a7f0-41e5-915f-1906a5bbb183)
![9 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/ae07a0e0-89cc-4711-b8ed-2582b70b1cdb)


10. cd weekly-task-app--> ls -l--> npm start ![10](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/693837fc-68f8-4ffc-88b2-c3b33163ee19)


11. Goto browser--> public_ip:3000 ![11](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/ecfa80aa-93d5-4679-91f1-d71ce8adcfe4)


12. aws codecommit create-repository --repository-name guvi-weekly-task-repo ![12](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/7c9e3265-b9ee-4fce-9010-4914cda8dbc1)


13. git init--> git add . -->git remote add codecommit <repo-url>--> git commi	t -m “commit-msg”--> global configuration ![13](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/4c8c17a7-9d87-4dd8-802a-a10845e5b465)


14. git remote add codecommit <codecommit-repo-url> --> git push codecommit master ![14](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/777d634b-d027-4eaa-93fe-55c52c451d49)


15. codes are successfully pushed to CodeCommit Repo ![15](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/211087da-42e9-4bba-bd74-f0a3dbb2f75e)
![15 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/2d96e983-2303-484e-a5e8-473d0c5c52e4)


16. Goto CodeCommit--> Create_Repository--> Repo_Name--> Create. ![16](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/e45f7fef-6c00-45ad-978f-423595f7c2bc)
![16 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/a714d240-3eff-400e-8e1e-1dddc29e7976)


17. Goto to CodeBuild--> Create Project--> Project_Name--> Source_provider--> Repository-->Branch--> Next. ![17](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/133a0667-2576-4bcd-9e2d-43b902330272)


18. Now click on Start Build--> build is successful. ![18](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/2869b285-1049-4c57-9475-e0bfd5b0076f)


19. Goto Code Pipeline--> Create Pipeline--> Name-->Next-->Source_provider--> ![19](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/dbaa7804-937c-4f77-8639-e03678fcbaa9)
![19 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/399a5fc2-41ba-461d-9dfd-87e336b8db8a)
![19 2](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/dc15127a-3b5a-4c5e-8fd6-c4e771e17af5)


20. ls -l--> docker build -t guvi-task-app .  
docker images --> docker push gaurav4u/guvi-task-app:v1 
