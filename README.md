# ESGF Melbourne (dev)

## Data

Minimum daily temperatures over 10 years (1981-1990) in the city Melbourne, Australia.

![Daily temperature evolution](docs/pics/temperature_evolution.png "Daily Temperature Evolution")

## Objective

We want to build a model able to predict the **daily** temperature in Melbourne over the **next year**.

## Evaluation

Fit one or more models using the data strictly anterior to the evaluation years 
`t=1987`, `t=1988` and `t=1989` in order to predict the daily temperature 
during the year `t=1987`, `t=1988` and `t=1989` respectively.

### Results


<table>
    <thead>
        <tr>
            <th>Evaluation year</th>
            <th>Next 3 months</th>
            <th>Next 6 months</th>
            <th>Next 12 months</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1987</td>
            <td>0.0273</td>
            <td>0.0079</td>
            <td>0.0386</td>
        </tr>
        <tr>
            <td>1988</td>
            <td>0.0118</td>
            <td>0.0071</td>
            <td>0.0198</td>
        </tr>
        <tr>
            <td>1989</td>
            <td>0.0190</td>
            <td>0.0122</td>
            <td>0.0443</td>
        </tr>
    </tbody>
</table


Le model le plus précis est le model est k=6. 
Il serait cependant interessant de voir si une modification de l architecture du réseau puisse améliorer les modèles k=3 et k=12. Le k=12 etant peut etre un peu léger pour retenir une si grande fenetre.
