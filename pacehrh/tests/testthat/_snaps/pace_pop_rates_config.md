# Population rates configuration: Load and compute

    Code
      popRates <- pacehrh:::loadPopulationChangeRates(sheetName = "newPopValues")
    Message <simpleMessage>
      Loading population change rates sheet newPopValues

---

    Code
      popRates <- pacehrh:::loadPopulationChangeRates(sheetName = "badPopValues")
    Message <simpleMessage>
      Loading population change rates sheet badPopValues
      Out of order BandEnd values for (Fertility, F)
      Incomplete BandStart/BandEnd range (0, 98) for (Mortality, F)
      Gaps in BandStart/BandEnd sequence for (Mortality, M)

---

    Code
      popRates <- pacehrh:::loadPopulationChangeRates(sheetName = "badPopValues_2")
    Message <simpleMessage>
      Loading population change rates sheet badPopValues_2
    Warning <simpleWarning>
      Missing required columns in table: Type

---

    Code
      popRates <- pacehrh:::loadPopulationChangeRates(sheetName = "badPopValues_4")
    Message <simpleMessage>
      Loading population change rates sheet badPopValues_4
      Incomplete BandStart/BandEnd range (2, 98)

---

    Code
      popRates <- pacehrh:::loadPopulationChangeRates(sheetName = "badPopValues_3")
    Message <simpleMessage>
      Loading population change rates sheet badPopValues_3
