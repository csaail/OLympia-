create database with name Sports(same as the project) or change the connection string according to your database;
in the same database create 2 tables and update the database:

1)Ordertest:
CREATE TABLE [dbo].[Ordertest] (
    [Id]       VARCHAR (50) NOT NULL,
    [Name]     VARCHAR (50) NOT NULL,
    [Phone]    VARCHAR (50) NOT NULL,
    [Adress]   VARCHAR (50) NOT NULL,
    [Quantity] INT          NOT NULL,
    [item]     VARCHAR (50) NOT NULL,
    [category] VARCHAR (50) NOT NULL,
    PRIMARY KEY CLUSTERED ([Id] ASC)
);

2)addstock:
CREATE TABLE [dbo].[addstock] (
    [Item_Id]          INT          IDENTITY (1, 1) NOT NULL,
    [Category]         VARCHAR (50) NOT NULL,
    [Item_name]        VARCHAR (50) NOT NULL,
    [Item_quantity]    INT          NOT NULL,
    [one_item_price]   INT          NOT NULL,
    [Total_item_price] INT          NOT NULL,
    PRIMARY KEY CLUSTERED ([Item_Id] ASC)
);
