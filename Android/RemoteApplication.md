##Project L: Remote App
###Remote Application Class
==========

###This is the Remote Application Class.

So, What's going in this class is mainly setup code.

A check to see if the device is connected to the internet via wifi or 3g/4g.

#####TODO: Also a check to see if the device is connected to bluetooth access

The instruction to check whether this device/user has already been registered is here. Basically,
a query is made to Usergrid to check if the remoteid which is a combination of the device's androidID and the device's
Mac Address, has been already stored and attributed to a record in the database. A flag is raised and 
stored in shared preferences indicating whether or not the device is registered. 

```java
    public Boolean getisRegistered() {
        return sharedPrefs.getBoolean(registered, false);
    }

    public void setisRegistered(Boolean isRegistered) {
        editor.putBoolean(registered, isRegistered).commit();
    }
```

```java
                            List<Entity> users = response.getEntities();
                            if (users.size() > 0) {
                                kvstore.setisRegistered(true);
                            } else {
                                kvstore.setisRegistered(false);
                            }
```




