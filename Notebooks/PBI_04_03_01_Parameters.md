WIP...

Dev(dataset) > PBI Service

Server name: rritec
Databasename: Adventureworksdw2012


Test

Server name: rritec_test
Databasename: Adventureworksdw2012_test


Prod

Server name: rritec_prod
Databasename: Adventureworksdw2012_prod

let
    Source = Sql.Database("rritec", "AdventureWorksDW2012"),
    dbo_DimDate = Source{[Schema="dbo",Item="DimDate"]}[Data]
in
    dbo_DimDate


let
    Source = Sql.Database(ServerName, DBName),
    dbo_DimDate = Source{[Schema="dbo",Item="DimDate"]}[Data]
in
    dbo_DimDate

let
    Source = Sql.Database("rritec", "AdventureWorksDW2012"),
    dbo_DimCustomer = Source{[Schema="dbo",Item="DimCustomer"]}[Data]
in
    dbo_DimCustomer

let
    Source = Sql.Database("rritec", "AdventureWorksDW2012"),
    dbo_FactInternetSales = Source{[Schema="dbo",Item="FactInternetSales"]}[Data],
    #"Filtered Rows" = Table.SelectRows(dbo_FactInternetSales, each [OrderDate] >= RangeStart and [OrderDate] <= RangeEnd)
in
    #"Filtered Rows"
