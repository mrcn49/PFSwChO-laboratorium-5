# PFSwChO-laboratorium-5

## Utworzenie przestrzeni nazw
<img width="419" height="336" alt="image" src="https://github.com/user-attachments/assets/fa6771ea-7a8c-4129-ad6b-87af202afe3b" />

## Zawartość plików quota
### dev-quota.yaml
<img width="474" height="393" alt="image" src="https://github.com/user-attachments/assets/bf101e26-27ca-468a-a57b-e645c0fe237a" />

### prod-quota.yaml
<img width="442" height="367" alt="image" src="https://github.com/user-attachments/assets/95ca8b4d-8141-4714-9748-8eade541c1af" />

## Zawartość pliku LimitRange
<img width="400" height="502" alt="image" src="https://github.com/user-attachments/assets/2aaa3b17-188f-4076-893c-efe637bdb723" />


## Uruchomienie plików:
<img width="408" height="201" alt="image" src="https://github.com/user-attachments/assets/392a92ba-8353-4fa4-83bb-60c31ba1e62c" />

## Weryfikacja:
<img width="965" height="446" alt="image" src="https://github.com/user-attachments/assets/81564028-9bfa-4b23-978e-e06a9616cf37" />

## Deployment no-test

### Generowanie bazowego pliku YAML
```
kubectl create deploy no-test --image=nginx -n ns-dev --dry-run=client -o yaml > deploy-no-test.yaml
```
### Zawartość pliku deploy-no-test.yml po modyfikacji
<img width="402" height="761" alt="image" src="https://github.com/user-attachments/assets/0e2b8c0e-ffb0-4da8-a3c5-d9dd9c47654d" />

### Uruchomienie pliku i weryfikacja:
<img width="763" height="317" alt="image" src="https://github.com/user-attachments/assets/a5e4ffbd-51e2-44a9-a56b-b1fce11cbc1b" />

### Wycinek wyniku polecenia kubectl describe rs no-test-75c4c789cb -n ns-dev potwierdzający poprawność wykonania zadania 
<img width="966" height="537" alt="image" src="https://github.com/user-attachments/assets/175d14da-c485-48f9-85be-ab4e2f227fa6" />

## Deployment yes-test
### Generowanie bazowego pliku YAML
```
kubectl create deploy yes-test --image=nginx -n ns-dev --dry-run=client -o yaml > deploy-yes-test.yaml
```
### Zawartość pliku deploy-yes-test.yml po modyfikacji
<img width="953" height="768" alt="image" src="https://github.com/user-attachments/assets/e9dc5e22-2187-4f00-8cfe-8495498d6cd9" />

### Uruchomienie pliku i weryfikacja:
<img width="962" height="338" alt="image" src="https://github.com/user-attachments/assets/d0a3ace8-a3fe-42ba-b267-f3decd191bef" />


## Deployment zero-test
### Generowanie bazowego pliku YAML

```
kubectl create deploy zero-test --image=nginx -n ns-dev --dry-run=client -o yaml > deploy-zero-test.yaml
```

### Zawartosc pliku deploy-zero-test.yml
<img width="965" height="632" alt="image" src="https://github.com/user-attachments/assets/96766897-25aa-47bf-a1d4-00d44e81d37d" />

### Uruchomienie pliku i weryfikacja
<img width="634" height="167" alt="image" src="https://github.com/user-attachments/assets/ab1bde5e-8c8f-4f04-b105-2697edb89348" />

### Wycinek polecenia kubectl describe pod zero-test-645589f969-fwgcs -n ns-dev potwierdzający poprawność wykonania zadania

<img width="968" height="460" alt="image" src="https://github.com/user-attachments/assets/02f49932-f6e2-46bb-8341-4df6d52b52a3" />

