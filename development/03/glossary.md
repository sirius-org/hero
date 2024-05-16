|                       | **Term**                 | **Definition**                                                                                                                                                                                            | **Note**                |
|-----------------------|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------|
| **Classes**           |                          |                                                                                                                                                                                                           |                         |
|                       | `AnalysisDescription`         | An activity that involves the quantification of risks to understand their magnitude and potential impact with respect to an asset.                                                                                                                             |                         |
|                       | `HeritageAsset`          | A physical or tangible item, structure, site, or object that holds historical, cultural, architectural, archaeological, or artistic significance and is considered worthy of preservation and protection. |                         |
|                       | `Risk`                   | The possibility of a loss of value to the heritage asset.                                                                                                                                                 |                         |
|                       | `Measure`              | A quantifiable aspect of something that expresses a more precise and standardised evaluation of it, based on assigning numerical values or metrics to some specific attributes.                                                                                                                                                                   |                         |
|                       | `Frequency`          | The measure representing the occurrence of the risk over time.                                                                                           | Subclass of `Measure` |
|                       | `FractionalValueLoss`          | The measure representing the loss of value expected in each item of the asset affected by the risk.                                                                                           | Subclass of `Measure` |
|                       | `Exposure`          | The measure representing the percentage or fraction of the heritage asset value that will be affected by the risk.                                                                                           | Subclass of `Measure` |
|                       | `Magnitude`          | The measure representing the overall impact and severity of a risk.                                                                                          | Subclass of `Measure` |
|                       | `Document`        | A source of knowledge that documents something.                                                                                                                                              |                         |
|                       | `TimeInterval`          | A period of time defined by a start date and a end date.                                                                                                                                                                |          |
| **Object properties** |                          |                                                                                                                                                                                                           |                         |
|                       | `describes`          | A property that links an analysis description to an asset.                                                                                                                                              |                         |
|                       | `analyses`            | A property that links an analysis description to a risk.                                                                                                                                                        |                         |
|                       | `isDocumentedBy`         | A property that links something to a document.                                                                                                                                             |                         |
|                       | `quantifies`           | A property that links an analysis description to a measure.                                                                                                                                                         |                         |
|                       | `atTime`           | A property that links an analysis description to a time interval.                                                                                                                                                       |                         |
| **Data properties**   |                          |                                                                                                                                                                                                           |                         |
|                       | `hasNote`                | A property that assigns a textual description to something.                                                                                                                                            |                         |
|                       | `hasLowEstimate`         | A property that assigns a estimate value for the best case scenario to a measure.                                                                                                                      |                         |
|                       | `hasProbableEstimate`    | A property that assigns a estimate value for the most likely case scenario to a measure.                                                                                                               |                         |
|                       | `hasHighEstimate`        | A property that assigns a estimate value for the worst case scenario to a measure.                                                                                                                     |                         |
|                       | `hasStartDate`                | A property that assigns a start date to a time interval.                                                                                                                                                                                 |          |
|                       | `hasEndDate`                | A property that assigns a end date to a time interval.                                                                                                                                                                                 |          |