# Database Queries

## find all customers that live in London. Returns 6 records.
    SELECT * FROM Customers where city is 'London'

    4	Around the Horn	Thomas Hardy	120 Hanover Sq.	London	WA1 1DP	UK
    11	B's Beverages	Victoria Ashworth	Fauntleroy Circus	London	EC2 5NT	UK
    16	Consolidated Holdings	Elizabeth Brown	Berkeley Gardens 12 Brewery	London	WX1 6LT	UK
    19	Eastern Connection	Ann Devon	35 King George	London	WX3 6FW	UK
    53	North/South	Simon Crowther	South House 300 Queensbridge	London	SW7 1RZ	UK
    72	Seven Seas Imports	Hari Kumar	90 Wadhurst Rd.	London	OX15 4NB	UK

## find all customers with postal code 1010. Returns 3 customers.
    SELECT * FROM Customers where postalcode is 1010

    12	Cactus Comidas para llevar	Patricio Simpson	Cerrito 333	Buenos Aires	1010	Argentina
    54	Océano Atlántico Ltda.	Yvonne Moncada	Ing. Gustavo Moncada 8585 Piso 20-A	Buenos Aires	1010	Argentina
    64	Rancho grande	Sergio Gutiérrez	Av. del Libertador 900	Buenos Aires	1010	Argentina

## find the phone number for the supplier with the id 11. Should be (010) 9984510.
    SELECT * FROM [Suppliers] where supplierid is 11

    11	Heli Süßwaren GmbH & Co. KG	Petra Winkler	Tiergartenstraße 5	Berlin	10785	Germany	(010) 9984510

## list orders descending by the order date. The order with date 1997-02-12 should be at the top.
    SELECT * FROM [Orders] order by orderdate desc

    10443	66	8	1997-02-12	1
    10442	20	3	1997-02-11	2
    10440	71	4	1997-02-10	2
    10441	55	3	1997-02-10	2
    10439	51	6	1997-02-07	3
    10438	79	3	1997-02-06	2
    10436	7	3	1997-02-05	2
    10437	87	8	1997-02-05	1
    10435	16	8	1997-02-04	2
    10433	60	3	1997-02-03	3
    10434	24	3	1997-02-03	2
    10432	75	3	1997-01-31	2
    10430	20	4	1997-01-30	1
    10431	10	4	1997-01-30	2
    10429	37	3	1997-01-29	2
    10428	66	7	1997-01-28	1
    10426	29	4	1997-01-27	1
    10427	59	4	1997-01-27	2
    10425	41	6	1997-01-24	2
    10423	31	6	1997-01-23	3
    10424	51	7	1997-01-23	2
    10422	27	2	1997-01-22	1
    10420	88	3	1997-01-21	1
    10421	61	8	1997-01-21	1
    10419	68	4	1997-01-20	2
    10418	63	4	1997-01-17	1
    10416	87	8	1997-01-16	3
    10417	73	4	1997-01-16	3
    10415	36	3	1997-01-15	1
    10413	41	3	1997-01-14	2
    10414	21	2	1997-01-14	3
    10412	87	8	1997-01-13	2
    10410	10	3	1997-01-10	3
    10411	10	9	1997-01-10	3
    10409	54	3	1997-01-09	1
    10408	23	8	1997-01-08	1
    10406	62	7	1997-01-07	1
    10407	56	2	1997-01-07	2
    10405	47	1	1997-01-06	1
    10403	20	4	1997-01-03	3
    10404	49	2	1997-01-03	1
    10402	20	8	1997-01-02	2
    10400	19	1	1997-01-01	3
    10401	65	1	1997-01-01	1
    10399	83	8	1996-12-31	3
    10398	71	2	1996-12-30	3
    10396	25	1	1996-12-27	3
    10397	60	5	1996-12-27	1
    10395	35	6	1996-12-26	1
    10393	71	1	1996-12-25	3
    10394	36	1	1996-12-25	3
    10392	59	2	1996-12-24	3
    10390	20	6	1996-12-23	1
    10391	17	3	1996-12-23	3
    10389	10	4	1996-12-20	2
    10388	72	2	1996-12-19	1
    10386	21	9	1996-12-18	3
    10387	70	1	1996-12-18	2
    10385	75	1	1996-12-17	2
    10383	4	8	1996-12-16	3
    10384	5	3	1996-12-16	3
    10382	20	4	1996-12-13	1
    10380	37	8	1996-12-12	3
    10381	46	3	1996-12-12	3
    10379	61	2	1996-12-11	1
    10378	24	5	1996-12-10	3
    10376	51	1	1996-12-09	2
    10377	72	1	1996-12-09	3
    10375	36	3	1996-12-06	2
    10373	37	4	1996-12-05	3
    10374	91	1	1996-12-05	3
    10372	62	5	1996-12-04	2
    10370	14	6	1996-12-03	2
    10371	41	1	1996-12-03	1
    10369	75	8	1996-12-02	2
    10368	20	2	1996-11-29	2
    10366	29	8	1996-11-28	2
    10367	83	7	1996-11-28	3
    10365	3	3	1996-11-27	2
    10363	17	4	1996-11-26	3
    10364	19	1	1996-11-26	1
    10362	9	3	1996-11-25	1
    10360	7	4	1996-11-22	3
    10361	63	1	1996-11-22	2
    10359	72	5	1996-11-21	3
    10358	41	5	1996-11-20	1
    10357	46	1	1996-11-19	3
    10356	86	6	1996-11-18	2
    10355	4	6	1996-11-15	1
    10354	58	8	1996-11-14	3
    10353	59	7	1996-11-13	3
    10352	28	3	1996-11-12	3
    10350	41	6	1996-11-11	2
    10351	20	1	1996-11-11	1
    10349	75	7	1996-11-08	1
    10348	86	4	1996-11-07	2
    10347	21	4	1996-11-06	3
    10346	65	3	1996-11-05	3
    10345	63	2	1996-11-04	2
    10344	89	4	1996-11-01	2
    10343	44	4	1996-10-31	1
    10342	25	4	1996-10-30	2
    10340	9	1	1996-10-29	3
    10341	73	7	1996-10-29	3
    10339	51	2	1996-10-28	2
    10338	55	4	1996-10-25	3
    10337	25	4	1996-10-24	3
    10336	60	7	1996-10-23	2
    10335	37	7	1996-10-22	2
    10334	84	8	1996-10-21	2
    10333	87	5	1996-10-18	3
    10332	51	3	1996-10-17	2
    10330	46	3	1996-10-16	1
    10331	9	9	1996-10-16	1
    10329	75	4	1996-10-15	2
    10328	28	4	1996-10-14	3
    10327	24	2	1996-10-11	1
    10326	8	4	1996-10-10	2
    10325	39	1	1996-10-09	3
    10324	71	9	1996-10-08	1
    10323	39	4	1996-10-07	1
    10322	58	7	1996-10-04	3
    10320	87	5	1996-10-03	3
    10321	38	3	1996-10-03	2
    10319	80	7	1996-10-02	3
    10318	38	8	1996-10-01	2
    10317	48	6	1996-09-30	1
    10316	65	1	1996-09-27	3
    10315	38	4	1996-09-26	2
    10314	65	1	1996-09-25	2
    10313	63	2	1996-09-24	2
    10312	86	2	1996-09-23	2
    10310	77	8	1996-09-20	2
    10311	18	1	1996-09-20	3
    10309	37	3	1996-09-19	1
    10308	2	7	1996-09-18	3
    10307	48	2	1996-09-17	2
    10306	69	1	1996-09-16	3
    10305	55	8	1996-09-13	3
    10304	80	1	1996-09-12	2
    10303	30	7	1996-09-11	2
    10302	76	4	1996-09-10	2
    10300	49	2	1996-09-09	2
    10301	86	8	1996-09-09	2
    10299	67	4	1996-09-06	2
    10298	37	6	1996-09-05	2
    10297	7	5	1996-09-04	2
    10296	46	6	1996-09-03	1
    10295	85	2	1996-09-02	2
    10294	65	4	1996-08-30	2
    10293	80	1	1996-08-29	3
    10292	81	1	1996-08-28	2
    10290	15	8	1996-08-27	1
    10291	61	6	1996-08-27	2
    10289	11	7	1996-08-26	3
    10288	66	4	1996-08-23	1
    10287	67	8	1996-08-22	3
    10286	63	8	1996-08-21	3
    10285	63	1	1996-08-20	2
    10284	44	4	1996-08-19	1
    10283	46	3	1996-08-16	3
    10282	69	4	1996-08-15	1
    10280	5	2	1996-08-14	1
    10281	69	4	1996-08-14	1
    10279	44	8	1996-08-13	2
    10278	5	8	1996-08-12	2
    10277	52	2	1996-08-09	3
    10276	80	8	1996-08-08	3
    10275	49	1	1996-08-07	1
    10274	85	6	1996-08-06	1
    10273	63	3	1996-08-05	3
    10272	65	6	1996-08-02	2
    10270	87	1	1996-08-01	1
    10271	75	6	1996-08-01	2
    10269	89	5	1996-07-31	1
    10268	33	8	1996-07-30	3
    10267	25	4	1996-07-29	1
    10266	87	3	1996-07-26	3
    10265	7	2	1996-07-25	1
    10264	24	6	1996-07-24	3
    10263	20	9	1996-07-23	3
    10262	65	8	1996-07-22	3
    10260	55	4	1996-07-19	1
    10261	61	4	1996-07-19	2
    10259	13	4	1996-07-18	3
    10258	20	1	1996-07-17	1
    10257	35	4	1996-07-16	3
    10256	88	3	1996-07-15	2
    10255	68	9	1996-07-12	3
    10254	14	5	1996-07-11	2
    10253	34	3	1996-07-10	2
    10252	76	4	1996-07-09	2
    10250	34	4	1996-07-08	2
    10251	84	3	1996-07-08	1
    10249	81	6	1996-07-05	1
    10248	90	5	1996-07-04	3

## find all suppliers who have names longer than 20 characters. You can use `length(SupplierName)` to get the length of the name. Returns 11 records.
    SELECT * FROM [Suppliers] where length(SupplierName) > 20

    2	New Orleans Cajun Delights	Shelley Burke	P.O. Box 78934	New Orleans	70117	USA	(100) 555-4822
    3	Grandma Kelly's Homestead	Regina Murphy	707 Oxford Rd.	Ann Arbor	48104	USA	(313) 555-5735
    5	Cooperativa de Quesos 'Las Cabras'	Antonio del Valle Saavedra	Calle del Rosal 4	Oviedo	33007	Spain	(98) 598 76 54
    8	Specialty Biscuits, Ltd.	Peter Wilson	29 King's Way	Manchester	M14 GSD	UK	(161) 555-4448
    10	Refrescos Americanas LTDA	Carlos Diaz	Av. das Americanas 12.890	São Paulo	5442	Brazil	(11) 555 4640
    11	Heli Süßwaren GmbH & Co. KG	Petra Winkler	Tiergartenstraße 5	Berlin	10785	Germany	(010) 9984510
    12	Plutzer Lebensmittelgroßmärkte AG	Martin Bein	Bogenallee 51	Frankfurt	60439	Germany	(069) 992755
    13	Nord-Ost-Fisch Handelsgesellschaft mbH	Sven Petersen	Frahmredder 112a	Cuxhaven	27478	Germany	(04721) 8713
    14	Formaggi Fortini s.r.l.	Elio Rossi	Viale Dante, 75	Ravenna	48100	Italy	(0544) 60323
    18	Aux joyeux ecclésiastiques	Guylène Nodier	203, Rue des Francs-Bourgeois	Paris	75004	France	(1) 03.83.00.68
    19	New England Seafood Cannery	Robb Merchant	Order Processing Dept. 2100 Paul Revere Blvd.	Boston	02134	USA	(617) 555-3267

## find all customers that include the word "market" in the name. Should return 4 records.
    SELECT * FROM [Customers] where customername like '%market%'

    10	Bottom-Dollar Marketse	Elizabeth Lincoln	23 Tsawassen Blvd.	Tsawassen	T2F 8M4	Canada
    32	Great Lakes Food Market	Howard Snyder	2732 Baker Blvd.	Eugene	97403	USA
    71	Save-a-lot Markets	Jose Pavarotti	187 Suffolk Ln.	Boise	83720	USA
    89	White Clover Markets	Karl Jablonski	305 - 14th Ave. S. Suite 3B	Seattle	98128	USA

## add a customer record for _"The Shire"_, the contact name is _"Bilbo Baggins"_ the address is _"1 Hobbit-Hole"_ in _"Bag End"_, postal code _"111"_ and the country is _"Middle Earth"_.
    insert into customers values (92, 'The Shire', 'Bilbo Baggins', '1 Hobbit-Hole', 'Bag End', 111, 'Middlw Earth')

    You have made changes to the database. Rows affected: 1

## update _Bilbo Baggins_ record so that the postal code changes to _"11122"_.
    update customers set postalcode = 11122 where customerid = 'Bilbo Baggings'

    You have made changes to the database.

## list orders grouped by customer showing the number of orders per customer. _Rattlesnake Canyon Grocery_ should have 7 orders.
    SELECT * FROM [Orders] left join customers on orders.CustomerID = Customers.CustomerID where customername = 'Rattlesnake Canyon Grocery'

    10262	65	8	1996-07-22	3	Rattlesnake Canyon Grocery	Paula Wilson	2817 Milton Dr.	Albuquerque	87110	USA
    10272	65	6	1996-08-02	2	Rattlesnake Canyon Grocery	Paula Wilson	2817 Milton Dr.	Albuquerque	87110	USA
    10294	65	4	1996-08-30	2	Rattlesnake Canyon Grocery	Paula Wilson	2817 Milton Dr.	Albuquerque	87110	USA
    10314	65	1	1996-09-25	2	Rattlesnake Canyon Grocery	Paula Wilson	2817 Milton Dr.	Albuquerque	87110	USA
    10316	65	1	1996-09-27	3	Rattlesnake Canyon Grocery	Paula Wilson	2817 Milton Dr.	Albuquerque	87110	USA
    10346	65	3	1996-11-05	3	Rattlesnake Canyon Grocery	Paula Wilson	2817 Milton Dr.	Albuquerque	87110	USA
    10401	65	1	1997-01-01	1	Rattlesnake Canyon Grocery	Paula Wilson	2817 Milton Dr.	Albuquerque	87110	USA

    SELECT * FROM [Orders] left join customers on orders.CustomerID = Customers.CustomerID order by Orders.CustomerID 

## list customers names and the number of orders per customer. Sort the list by number of orders in descending order. _Ernst Handel_ should be at the top with 10 orders followed by _QUICK-Stop_, _Rattlesnake Canyon Grocery_ and _Wartian Herkku_ with 7 orders each.

    SELECT Customers.CustomerName, count(Orders.CustomerID) as OrderIds FROM [Orders] left join customers on orders.CustomerID = Customers.CustomerID group by Orders.CustomerID order by OrderIds desc


## list orders grouped by customer's city showing number of orders per city. Returns 58 Records with _Aachen_ showing 2 orders and _Albuquerque_ showing 7 orders.

   SELECT Customers.City, count(Orders.CustomerID) as OrderIds FROM [Orders] left join customers on orders.CustomerID = Customers.CustomerID group by Customers.City order by OrderIDs desc

## delete all users that have no orders. Should delete 17 (or 18 if you haven't deleted the record added) records.

    delete from Customers where not exists (select CustomerId from Orders where customerID = Customers.CustomerID)

    You have made changes to the database. Rows affected: 18