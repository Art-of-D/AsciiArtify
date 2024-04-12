# MVP

---

1. So after you create your app you need to check it:

2. Next, check the work of k3d and connect `k port-forward -n demo svc/ambassador 8081:80&`. But you can use another port than 8081, but do not use 8080 if you used it for connection to argo cd GUI.
   ![](check.gif)
3. Now you can work with your app. But do not forget to do it in another terminal window after connection.
   ![](last.gif)
