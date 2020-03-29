# Label-ouside-of-rim-
This article explains about how to show the label in the outside of rim in Xamarin Circular Gauge. Please refer KB links for more details,

[How to show labels and ticks outside the rim in Xamarin.Forms Radial Gauge](https://www.syncfusion.com/kb/11283/how-to-show-labels-and-ticks-outside-the-rim-in-xamarin-forms-radial-gauge)

By adjusting the Offset property of [**Scale**](https://help.syncfusion.com/cr/xamarin/Syncfusion.SfGauge.XForms~Syncfusion.SfGauge.XForms.Scale.html), [**TickSettings**](https://help.syncfusion.com/cr/xamarin/Syncfusion.SfGauge.XForms~Syncfusion.SfGauge.XForms.TickSettings.html), and [**Range**](https://help.syncfusion.com/cr/xamarin/Syncfusion.SfGauge.XForms~Syncfusion.SfGauge.XForms.Range.html) values, we can display the circular gauge labels on the outside of its rim. 

**XAML:**

```

    <gauge:SfCircularGauge x:Name="circularGauge" >
        <gauge:SfCircularGauge.Scales>
            <gauge:Scale StartAngle="180" SweepAngle="180" ShowLabels="True" ShowRim="True"
                   StartValue="0" EndValue="150" Interval="30" RimColor="#e0e0e0"
           RadiusFactor="0.83" RimThickness="40"    LabelOffset="0.95" ScaleStartOffset="0.83" ScaleEndOffset="0.73">

                <gauge:Scale.Pointers>
                    <gauge:NeedlePointer KnobRadius="0" Value="10" KnobStrokeColor="#0682F6" KnobStrokeWidth="6"
                                        Color="#F67E09"  KnobColor="White" Type="Triangle" Thickness="10" LengthFactor="0.66"/>
                </gauge:Scale.Pointers>

                <gauge:Scale.MajorTickSettings>
                    <gauge:TickSettings StartOffset="0.83" EndOffset="0.90" Thickness="2"/>
                </gauge:Scale.MajorTickSettings>
                <gauge:Scale.MinorTickSettings>
                    <gauge:TickSettings StartOffset="0.83" EndOffset="0.88" Thickness="2"/>
                </gauge:Scale.MinorTickSettings>
                <gauge:Scale.Ranges>
                    <gauge:Range StartValue = "0" EndValue = "10" Color = "#F67E09" Thickness = "40" Offset = "0.83" />
                </gauge:Scale.Ranges>
            </gauge:Scale>
        </gauge:SfCircularGauge.Scales>
    </gauge:SfCircularGauge>

```

**See also:**

[How do I set the start and end values for the scale?](https://help.syncfusion.com/xamarin/circular-gauge/scales#setting-start-and-end-values-for-scale)

[How do I customize the position of rim?](https://help.syncfusion.com/xamarin/circular-gauge/rim#setting-position-for-rim)

[How do I add a needle pointer to the gauge?](https://help.syncfusion.com/xamarin/circular-gauge/pointers#needle-pointer)

[How to change the position of ticks?](https://help.syncfusion.com/xamarin/circular-gauge/tick-setting#setting-position-for-ticks)

Also refer our [feature tour](https://www.syncfusion.com/xamarin-ui-controls/xamarin-circular-gauge) page to know more features available in our SfCircularGauge.

## <a name="troubleshooting"></a>Troubleshooting ##
### Path too long exception
If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.

