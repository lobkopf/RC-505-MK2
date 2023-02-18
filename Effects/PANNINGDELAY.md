# GRANUALR DELAY

## Official documentation
>This delay is specifically for stereo output. This allows you to obtain the tap delay
effect that divides the delay time, then deliver them to L and R channels.
>
>| Parameter | Value (Bold: default) | Explanation |
>| --------- | --------------------- | ----------- |
>| Time       | 0 - **200** - 2000, 1/2-note - 1/32-note      | Sets the delay time. |
>| Feedback  | 0 - **16**  `*`   | Sets the numbers of delay repeats. |
>| D.Level | 0 - **100**      | Sets the volume of the direct sound. |
>| Low Cut | **FLAT**, 20.0 Hz - 12,5 Hz | Sets the frequency at which the low cut filter begins to take effect. When “FLAT” is selected, the low cut filter will have no effect. |
>| Low Cut | 20.0 Hz - 12,5 Hz, **FLAT** | Sets the frequency at which the high cut filter begins to take effect. When “FLAT” is selected, the high cut filter will have no effect. |
>| E-Level `KNOB`  | 0 - **50** - 120      | Sets the volume of the delay sound. |

`*` The official documentation is wrong regarding this parameter. In actuality values for `Feedback` are (0 - **20** - 100).

## Additional documentation
#### Note Values
As pitch is only a certain frequency, a delay can be used to generate a pitched note when using an appropriately small `Time`.
The relation of the pitch/frequency and the `Time` is:\
$1 ms = 1 * 10^(-3) s = 1/(1 * 10^(-3)) Hz$
The resulting frequencies are listed in the table above.
Furthermore the table lists the closest "normal" note (`Relative Note`) and the "target" frequency of that note (`Frequency of the Note`) ([12-TET](https://en.wikipedia.org/wiki/12_equal_temperament)) with A4 at 440 Hz.
The results are listed until C0 because lower values are no longer suitable to produce audible pitches as their frequency is too low (arguably this cut-off could be higher).

|`Time` in ms|`Time` in s|Pitch/Frequency in Hz|Relative Note|Frequency of the Note|
|:----|:----|:----|:----|:----|
|1|0,001|1000|C6|1046,5020|
|2|0,002|500|B4|493,8833|
|3|0,003|333,3333333|E4|329,6276|
|4|0,004|250|B3|246,9417|
|5|0,005|200|G3|195,9977|
|6|0,006|166,6666667|E3|164,8138|
|7|0,007|142,8571429|D3|146,8324|
|8|0,008|125|B2|123,4708|
|9|0,009|111,1111111|A2|110,0000|
|10|0,01|100|G2|97,9989|
|11|0,011|90,90909091|F♯2/G♭2|92,4986|
|12|0,012|83,33333333|E2|82,4069|
|13|0,013|76,92307692|D♯2/E♭2|77,7818|
|14|0,014|71,42857143|C♯2/D♭2|69,2957|
|15|0,015|66,66666667|C2/Deep C|65,4064|
|16|0,016|62,5|B1|61,7354|
|17|0,017|58,82352941|A♯1/B♭1|58,2705|
|18|0,018|55,55555556|A1|55,0000|
|19|0,019|52,63157895|G♯1/A♭1|51,9131|
|20|0,02|50|G1|48,9994|
|21|0,021|47,61904762|F♯1/G♭1|46,2493|
|22|0,022|45,45454545|F♯1/G♭1|46,2493|
|23|0,023|43,47826087|F1|43,6535|
|24|0,024|41,66666667|E1|41,2034|
|25|0,025|40|D♯1/E♭1|38,8909|
|26|0,026|38,46153846|D♯1/E♭1|38,8909|
|27|0,027|37,03703704|D1|36,7081|
|28|0,028|35,71428571|D1|36,7081|
|29|0,029|34,48275862|C♯1/D♭1|34,6478|
|30|0,03|33,33333333|C1/Pedal C|32,7032|
|31|0,031|32,25806452|C1 Pedal C|32,7032|
|32|0,032|31,25|B0|30,8677|
|33|0,033|30,3030303|B0|30,8677|
|34|0,034|29,41176471|A♯0/B♭0|29,1352|
|35|0,035|28,57142857|A♯0/B♭0|29,1352|
|36|0,036|27,77777778|A0|27,5000|
|37|0,037|27,02702703|A0|27,5000|
|38|0,038|26,31578947|G♯0/A♭0|25,9565|
|39|0,039|25,64102564|G♯0/A♭0|25,9565|
|40|0,04|25|G0|24,4997|
|41|0,041|24,3902439|G0|24,4997|
|42|0,042|23,80952381|F♯0/G♭0|23,1247|
|43|0,043|23,25581395|F♯0/G♭0|23,1247|
|44|0,044|22,72727273|F♯0/G♭0|23,1247|
|45|0,045|22,22222222|F0|21,8268|
|46|0,046|21,73913043|F0|21,8268|
|47|0,047|21,27659574|F0|21,8268|
|48|0,048|20,83333333|E0|20,6017|
|49|0,049|20,40816327|E0|20,6017|
|50|0,05|20|D♯0/E♭0|19,4454|
|51|0,051|19,60784314|D♯0/E♭0|19,4454|
|52|0,052|19,23076923|D♯0/E♭0|19,4454|
|53|0,053|18,86792453|D0|18,3541|
|54|0,054|18,51851852|D0|18,3541|
|55|0,055|18,18181818|D0|18,3541|
|56|0,056|17,85714286|D0|18,3541|
|57|0,057|17,54385965|C♯0/D♭0|17,3239|
|58|0,058|17,24137931|C♯0/D♭0|17,3239|
|59|0,059|16,94915254|C♯0/D♭0|17,3239|
|60|0,06|16,66666667|C0/Double Pedal C|16,3516|
|61|0,061|16,39344262|C0/Double Pedal C|16,3516|
|62|0,062|16,12903226|C0/Double Pedal C|16,3516|
|63|0,063|15,87301587| | |
|64|0,064|15,625| | |
|65|0,065|15,38461538| | |
|66|0,066|15,15151515| | |
|67|0,067|14,92537313| | |
|68|0,068|14,70588235| | |
|69|0,069|14,49275362| | |
|70|0,07|14,28571429| | |
|71|0,071|14,08450704| | |
|72|0,072|13,88888889| | |
|73|0,073|13,69863014| | |
|74|0,074|13,51351351| | |
|75|0,075|13,33333333| | |
|76|0,076|13,15789474| | |
|77|0,077|12,98701299| | |
|78|0,078|12,82051282| | |
|79|0,079|12,65822785| | |
|80|0,08|12,5| | |
|81|0,081|12,34567901| | |
|82|0,082|12,19512195| | |
|83|0,083|12,04819277| | |
|84|0,084|11,9047619| | |
|85|0,085|11,76470588| | |
|86|0,086|11,62790698| | |
|87|0,087|11,49425287| | |
|88|0,088|11,36363636| | |
|89|0,089|11,23595506| | |
|90|0,09|11,11111111| | |
|91|0,091|10,98901099| | |
|92|0,092|10,86956522| | |
|93|0,093|10,75268817| | |
|94|0,094|10,63829787| | |
|95|0,095|10,52631579| | |
|96|0,096|10,41666667| | |
|97|0,097|10,30927835| | |
|98|0,098|10,20408163| | |
|99|0,099|10,1010101| | |
|100|0,1|10| | |
|101|0,101|9,900990099| | |
|102|0,102|9,803921569| | |

#### Assign
> `TARGET MIN` and `TARGET MAX`: Specifies the variable range of the function (parameter) that is specified as the target.
The value (MIN: minimum value, MAX: maximum value) depends on the parameter that is specified as the target.

##### Time
##### Feedback
##### D-Level
##### Low Cut
##### High Cut
##### E-Level

###### _Operationalization_
_GRANULAR DELAY in TFX AA, Inward Kick without any FX looped as trigger-sound. Comparison to the relative sine wave via <https://onlinetonegenerator.com/> done by ear for a few example sounds at different_ `Time` _values. Generalization of these values to the full table._ \
_Different trigger-sounds might contain different overtones, which might change/influence the pitch perception._
