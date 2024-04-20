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


18. Now click on Start Build build is successful. ![18](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/c314dc04-74a4-4553-8e02-a5077782a0ff)
![18 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/7d10e314-9cf5-42e7-bc36-468d9c2d8fe3)

 
19. Goto Elastic Beanstalk Create ApplicationNameCreate. ![19](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/928c1adb-0ce7-4a87-8496-a8541f6e73db)
![19 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/ac3c4950-b3f4-4943-82d0-dd4286e986f9)
![19 2](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/a0bf03b0-a33a-45ee-a591-ebe43e0cc748)


20. Click on created application Filling all details ReviewSubmit ![20](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/4afacb62-204f-4e12-9d30-1e6b8cc2bfaf)


21. Beanstalk environment createdsuccessfully launched beanstalk environment ![21](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/97d83caa-52d4-4a4f-95c9-ace7db2715c1)
![21 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/aae573b5-bd22-47af-a3b1-3f14b6f997c3)
 

22. Copy the public_ip of “Guvi-beanstalk-env-env” and paste it in browser. ![22](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/565348c5-e2a7-42bd-99e4-93ce9be9d654)


23. Goto Code Pipeline Create Pipeline Filled all details Review Submit ![23](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/78694ac4-f64f-4495-a83e-931a3efe4eb2)


24. Pipeline started Build  Deploy. ![24](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/3ef40d14-4ab6-41ae-b867-c48149d12514)
![24 1](https://github.com/GauravDevOps711/Weekly-Task/assets/135973657/aeb0c2d1-cafc-4c87-99a0-b5666968eb0a)

