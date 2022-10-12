# Managers

#### Reliability and availability[#](broken-reference) <a href="#reliability-and-availability" id="reliability-and-availability"></a>

Reliability and availability are two important metrics to measure compliance of service to agreed-upon service level objectives (SLO).

The measurement of availability is driven by time loss, whereas the frequency and impact of failures drive the measure of reliability. Availability and reliability are essential because they enable the stakeholders to assess the health of the service.

Reliability (`R`) and availability (`A`) are two distinct concepts, but they are related. Mathematically, `A` is a function of `R`. This means that the value of `R` can change independently, and the value of `A` depends on `R`. Therefore, it’s possible to have situations where we have:

* low `A`, low `R`
* low `A`, high `R`
* high `A`, low `R`
* high `A`, high `R` (desirable)
