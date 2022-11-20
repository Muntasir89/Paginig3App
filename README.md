# Paginig3App
The Paging library helps you load and display pages of data from a larger dataset from local storage or over network. This approach allows your app to use both network bandwidth and system resources more efficiently.
# Theory
**_PagingSource<Int,UnsplashImage>()_**</br>
**KEY:** Identifier used to load the data. Usually a Page number.</br>
**VALUE:** Type of the data that will be loaded and desplayed to the users.</br>
### Paging Data
**Paging Data** is a containerr for Paged data from a single generation of loads. </br></br>
**PagingSource** class is used when data is loaded from a single source (Database, Network or a File).</br>
**PagingSouce+RemoteMediator** is used when data is loaded from a layered source (Network Source + Database Cache). </br>
The main role of **RemoteMediator** is to load more data from the network either the page run out of the data or the existing data is invalidated.</br>
**Remote Keys** is the keys that **RemoteMediator** is using to tell the back-end service which data to load next. 
