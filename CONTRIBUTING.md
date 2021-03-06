## Contributing to CoordinateSharp
Any contribution to this library is greatly appreciated! Developers are encouraged to create issues, ask questions and fork this library. 
If you wish to contribute to the codebase, please follow the below guidelines. 

### Organization

The codebase is organized into various .cs files. If modifying the codebase, ensure you are familiar with how it is organized so that
items go into the proper file. 

* Coordinate.cs - Stores the `Coordinate` and `CoordinatePart` model, properties and change notifications.
* Coordinate.Assistant.cs - Handles additional logic and additional custom property types for all coordinate type models.
* Coordinate.UTM.cs - Handles UTM model and property types. Also contains conversion logic.
* Coordinate.MGRS.cs - Handles MGRS (NATO UTM) model and property types. Also contains conversion logic. MGRS logic relies upon the `UTM` class.
* Coordinate.Cartesian.cs - Handles Cartesian model and property types. Also contains conversion logic.
* Celestial.cs - Stores the `Celestial` model and properties.
* Celestial.Assistant.cs - Handles logic and custom property types for the `Celestial` model.
* Celestial.SunCalculations.cs - Handles all solar calculations (except eclipse).
* Celestial.MoonCalculation.cs - Handles all lunar calculations (except eclipse).
* Celestial.SolarEclipseCalc.cs - Handles solar eclipse calculations.
* Celestial.LunarEclipseCalc.cs - Handles lunar eclipse calculations.

### Readable Code

Please make code readable and easy to understand. Comment on any obscure object names or code.

### Testing

Developers are encouraged to write and share tests for changes made. Please use the automated testing project provided with the solution to verify changes. Forks will be tested both manually and automated prior to merging.

NOTE: Conversion Test PASS # 4 is currently failing. This is due to an incorrect MGRS conversion in a circumpolar region. An issue has been raised, and you may ignore that PASS at this time.

### Pull Requests

It is asked that you are clear in specifying **WHAT** you changed and **WHY**. With that said there is no formal template for pull requests.
You may however be asked to adjust code if organization doesn't flow or code isn't clear. If you plan to make changes to celestial calculations,
an explanation of the changes will be sought.

Please submit Pull Requests to the [Develop Branch](https://github.com/Tronald/CoordinateSharp/tree/Develop). The Master branch will only contain stable versions.

## Summary

That's it! Be creative and be innovative. All help is welcome and encouraged!
