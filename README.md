# Helm

this code deploy and run WordPress with helm.

## Usage

#### Add Helm repo :
```bash
helm repo add bitnami https://charts.bitnami.com/bitnami
```

![image](https://github.com/remaegbaria/helm/blob/main/add%20repo.png)

---

#### Install the chart with the release name my-release with adding smtpHost parametre :
```bash
helm install my-release bitnami/wordpress --set smtpHost=smtp.gmail.com
```

![image](https://github.com/remaegbaria/helm/blob/main/deploy-wordpress.png)

---

#### Check values :
```bash
helm get values my-release
```

![image](https://github.com/remaegbaria/helm/blob/main/values.png)

---

#### Check deployment in k8s :
```bash
kubectl get deployments
```

![image](https://github.com/remaegbaria/helm/blob/main/deploy-in-k8s.png)

---

#### Check services in k8s :
```bash
kubectl get services
```

![image](https://github.com/remaegbaria/helm/blob/main/services-in-k8s.png)

---
