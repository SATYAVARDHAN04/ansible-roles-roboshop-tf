# DEVELOPING ROBOSHOP PROJECT USING ANSIBLE ROLES 

## 1. MONGODB ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=mongodb main.yaml
```

## 2. CATALOGUE ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=catalogue main.yaml
```

## 3. MYSQL ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=mysql main.yaml
```

## 4. RABBITMQ ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=rabbitmq main.yaml
```

## 5. USER ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=user main.yaml
```

## 6. PAYMENT ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=payment main.yaml
```

## 7. CART ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=cart main.yaml
```

## 8. SHIPPING ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=shipping main.yaml
```

## 9. REDIS ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=redis main.yaml
```
## 10. FRONTEND ROLE

```bash
ansible-playbook -i inventory.ini -e componenet=frontend main.yaml
```


# WORKING WITH ANSIBLE VAULT

## 1. CREATING ANSIBLE VAULT

```bash
ansible-vault create filename.yaml
```

## 2. EDITING ANSIBLE VAULT

```bash
ansible-vault edit filename.yaml
```

## 3. VIEWING ANSIBLE VAULT

```bash
ansible-vault view filename.yaml
```

## 4. DELETING ANSIBLE VAULT

```bash
ansible-vault delete filename.yaml
```

## 5. CHANGING PASSWORD OF ANSIBLE VAULT

```bash
ansible-vault rekey filename.yaml
```
## AFTER SETTING VAULT PASSWORD AND FILES ON ec2 MACHINES RUN THIS COMMAND

```bash
ansible-playbook -i inventory.ini -e componenet=mysql mysql.yaml --ask-vault-pass
```
