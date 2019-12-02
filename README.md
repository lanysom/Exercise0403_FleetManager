# Exercise0403 FleetManager

You have expanded your business so you need more cars which makes it more complex to handle your fleet. Also you have more meetings which means you will not always be present at the office. So you hired an employee named Fritz to help you. This means you need to upgrade your system so it is able to handle that both you and Fritz can manage the cars. The additional requirements for your application are as follows:

1. When a car is registered as rented, the employee who handled it should be registered as well.
1. When a car is registered as returned, the employee who handled it should be registered as well.
1. The system should be able to handle at least two concurrent users.

First you need to upgrade your database so you can register who handles a car. Again you are free to do this yourself, but if you used the table defined in the previous exercise, you can add an employee column to that with the script below

```
ALTER TABLE [dbo].[Cars]
    ADD [Employee] NVARCHAR (50) NULL;
```

