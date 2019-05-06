### 1. 领域建模

------

- **Make Reservation**

  - 类图
    ![](https://github.com/qw1998/xitongfenxi/blob/master/pic/6_2.jpg)
    

  - 表结构

    ```sql
    [new.uxf](new.uxf) Customer(ID/key, FullName, EmailAdress)
    City(ID/key, Name)
    Hotel(ID/key, Name, Adress, CityID/Fkey)
    Room(RoomID/key, HotelID/Fkey, Type, Availability)
    ReservationItem(ID/key, RoomID/Fkey, BasketID/Fkey, checkInDate, checkOutDate, NumberOfAdults, NumberOfChildren, Price, IsSmoking)
    ReservationBasket(ID/key, CustomerID/Key)
    ```

-  **Payment**

  - 类图
    ![](https://github.com/qw1998/xitongfenxi/blob/master/pic/6_3.jpg)
    

  - 表结构

    ```sql
    Payment(ID/key, totalPrice, reservationID/Fkey, cardID/Fkey)
    ReservationItem(ID/key, paymentID/Fkey,checkInDate, ...)
    CreditCard(ID/key, Type, CardSecurityCode, ExpiryDate, CardHolderID/Fkey)
    CardHolder(ID/key, Title, FirstName, LastName, Address1, Address2, City, CountyOrState, Country, Postcode, DaytimeTelephone, EveningTelephone)
    ```

## ### . Reservation生命周期建模

![](https://github.com/qw1998/xitongfenxi/blob/master/pic/6_1.jpg)
