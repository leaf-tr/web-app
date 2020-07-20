# web-app
A repo that will keep submodules of front-end and back-end in one container

### Contributing
If you want to test both front-end and back-end as the whole system use this repo, otherwise use each respective submodule

to clone you need to need to add a recursive flag so folders within submodules will be cloned as well

`git clone --recurse-submodules https://github.com/leaf-tr/web-app`

To work on the project, you can `cd` into each submodule and create a new branch
```
cd front-end
git checkout -b "new-branch-name"
```

Inside the `front-end` or `back-end` folder you can run Docker:
```
docker-compose build
docker-compose up
```

If you want to add a new dependency for the back-end(in `requirements.txt`) or for the front-end(in `package.json`), you will have to rebuild Docker image
```
docker-compose build
docker-compose up
```

Work on your features and when ready to commit run typical commands:
```
git add .
git commit -m "Added new features"
git push
```
Create a pull request (PR) on the respective repository

