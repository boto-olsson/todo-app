# todo-app
1. Use oc create with the -f option against todo-db.yaml to deploy the database server pod
2. oc cp db-data.sql mysql-podname:/tmp/
3. oc rsh mysql-podname /bin/bash mysql -u root items < /tmp/db-data.sql
4. oc create -f todo-frontend.yaml
5. oc expose service frontend
