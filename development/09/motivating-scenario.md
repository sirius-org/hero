# Iteration 09

## Name
Dependence (motivation and use)

## Description
An assessment activity can be motivated by any kind of information element that serves as a scientific basis for that activity and the assertions it assigns to a cultural heritage object.

Moreover, an assertion activity may depend on the use of specific objects in order to be carried out (such as certain instrumentation, mathematical equations, algorithms, datasets, etc.).

## Example 01
An assessment activity `:assessment-activity-05`, consisting in the analysis of risks related to a CHO `:baptistery`, is taking place in Ravenna, is documented in the document `:document-03` and is being carried out by the expert Sara Fiorentino, in the time interval starting from 2024-04-01 to 2024-05-01, continuing `:assessment-activity-03`. It is annotated with the following text: "A flood event is expected in the baptistery approximately once every 25 years, most likely affecting the whole heritage asset value per event, resulting in a partial loss." It is composed of four statements, each assigned to the CHO in question:
1. `:observation-16`, which is a dimensions description referring to the frequency of the risk occurrence (`:concept-16`). In turn, the frequency is composed of three other concepts:
    * low estimate (`:concept-16a`), with a value of "3.0";
    * probable estimate (`:concept-16b`), with a value of "3.5";
    * high estimate (`:concept-16c`), with a value of "4.0".
2. `:observation-17`, which is a dimensions description referring to the fractional value loss determined by the risk occurrence (`:concept-17`). In turn, the fractional value loss is composed of three other concepts:
    * low estimate (`:concept-17a`), with a value of "4.5";
    * probable estimate (`:concept-17b`), with a value of "5.0";
    * high estimate (`:concept-17c`), with a value of "5.0".
3. `:observation-18`, which is a dimensions description referring to the exposure determined by the risk occurrence (`:concept-18`). In turn, the exposure is composed of three other concepts:
    * low estimate (`:concept-18a`), with a value of "1.5";
    * probable estimate (`:concept-18b`), with a value of "2.0";
    * high estimate (`:concept-18c`), with a value of "2.5".
4. `:observation-19`, which is a dimensions description referring to the magnitude of the risk occurrence (`:concept-19`). In turn, the magnitude is composed of three other concepts:
    * low estimate (`:concept-19a`), with a value of "9.0";
    * probable estimate (`:concept-19b`), with a value of "10.5";
    * high estimate (`:concept-19c`), with a value of "11.5".

This assessment activity uses `dati_subsidenza_2011-2016.zip` as a basis for its statements.

## Example 04
An assessment activity `:assessment-activity-07` consisting in the evaluation of risks related to a CHO `:baptistery`, is taking place in Ravenna and is being carried out by the expert Sara Fiorentino, in the time interval starting from 2024-05-01 to 2024-06-01, continuing `:assessment-activity-05`. It is annotated with the following text: "The risk of flood (MR = 10.5) has a high priority. It is 100 times smaller than the fire risk. The uncertainty that has been measured amounts to a value equal to 2.5. A risk of this magnitude is equivalent to losing about 0.3% of the heritage asset value every 100 years (or 3% per millennium). The museum direction considers this level of risk as just beyond acceptable, since as a condition the value of MR is slightly higher than 10 and the value of uncertainty is higher than 2." It consists of one statement assigned to the CHO in question:
1. `:observation-24`, which is a diagnosis referring to a high level of priority(`:concept-24`).

This assessment activity is motivated by the magnitude of the risk occurrence described in a previous activity (`:concept-19`).
