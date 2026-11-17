# Projeto28 – Car Rental Service

A Java exercise modelling a **car rental** system with a pluggable tax strategy.

## Status
Work in progress: the domain classes and services are scaffolded; the main program is not implemented yet.

## Structure
```
application.Projeto28
entities   CarRental, Vehicle, Invoice
services   RentalService, TaxService (interface), BrazilTaxService
```

## Idea
`RentalService` calculates the rental price (by hour or by day) and asks a `TaxService` for the tax, producing an `Invoice`. Because tax rules depend on the country, `TaxService` is an interface and `BrazilTaxService` is one implementation, illustrating interfaces and dependency inversion.

## Run
Requires JDK 17+. Open in IntelliJ IDEA and run `application.Projeto28`.
