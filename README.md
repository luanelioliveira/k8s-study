<h1 align="center">
    My Study K8S
</h1>

<h3 align="center">
  Learning Kubernetes Basics
</h3>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/luanelioliveira/k8s-study?color=%2304D361">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/luanelioliveira/k8s-study">

  <a href="https://www.linkedin.com/in/luanoliveira/" target="_blank">
    <img alt="Made by Luan Eli Oliveira" src="https://img.shields.io/badge/made%20by-Luan%20Eli%20Oliveira-brightgreen">
  </a>

  <a href="https://github.com/luanelioliveira/k8s-study/commits/master">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/luanelioliveira/k8s-study">
  </a>

  <a href="https://github.com/luanelioliveira/k8s-study/issues">
    <img alt="Repository issues" src="https://img.shields.io/github/issues/luanelioliveira/k8s-study">
  </a>

  <img alt="License" src="https://img.shields.io/badge/license-MIT-brightgreen">
</p>

<p align="center">
  <a href="#rocket-Technologies">Technologies</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-how-to-use">How to use</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-how-to-contribute">How to contribute</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-license">License</a>
</p>

<br>

## :rocket: Technologies

This project was developed as part of my study

- [Kubernetes](https://kubernetes.io/pt/)

## :desktop_computer: How to use

- Clone it: ```git clone https://github.com/luanelioliveira/k8s-study.git```
- Enter in the project:  ```cd k8s-study```
- Start your minikube: ```minikube start --driver=hyperkit```

Deploy to dev: 
```bash 
$ kubectl create -f samples/environments/dev/namespace.yaml --save-config --record
$ kubectl create -f samples/environments/dev --save-config --record
```

Deploy to sandbox: 
```bash 
$ kubectl create -f samples/environments/sandbox/namespace.yaml --save-config --record
$ kubectl create -f samples/environments/sandbox --save-config --record
```

Deploy to prod: 
```bash 
$ kubectl create -f samples/environments/prod/namespace.yaml --save-config --record
$ kubectl create -f samples/environments/prod --save-config --record
```

- Get ip minukube: ```minikube ip```
- Then open http://cluster-ip:30701/ to see your app.
- Connect postgres database http://cluster-ip:30700/ with database `postgres`, user `postgres` and password `postgres`

## 🤔 How to contribute

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
Please make sure to update tests as appropriate.

- Make a fork;
- Create a branck with your feature: `git checkout -b my-feature`;
- Commit changes: `git commit -m 'feat: My new feature'`;
- Make a push to your branch: `git push origin my-feature`.

After merging your receipt request to done, you can delete a branch from yours.

## :memo: License

This project is under the MIT license. See the [LICENSE](LICENSE) for details.

---
Made by Luan Eli Oliveira :wave: [Get in touch!](https://www.linkedin.com/in/luanoliveira/)