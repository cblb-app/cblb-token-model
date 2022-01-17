# CBLB token issue model - MATIC version - final

Inspired by **Torricelli's Trumpet**, appropriately increase the ratio and displacement parameter modification formula as the following form, and use the sign-in behavior as the only trigger condition for the issuance of CBLB Token.

![](https://raw.githubusercontent.com/cblb-app/cblb-token-model/master/imgs/GabrielHorn.png)

CBLB token issuance formula  
![](https://raw.githubusercontent.com/cblb-app/cblb-token-model/master/imgs/formula.svg)

The document `token-issue-model.ipynb` contains a simulation of the issuance chart of CBLB token.

Considering the two factors of smart contract interaction cost and block confirmation waiting time, cblb.app chooses polygon as the application backend.

To further refine the CBLB issuance model, CBLB will be set to be acquired only through sign-in behavior, and the sign-in needs to pay MATIC as a fee, and the number of MATIC required for each sign-in is fixed.

Check-in fee is fixed by formula

```
fee = 144600 / (100 + 100) / 6390 = 0.11314554 MATIC
```

The number of CBLBs obtained by check-in decreases with the total number of check-ins according to the model. This ensures that a stable and long-term positive exchange ratio is established between CBLB and MATIC.

**100 times check-in token issue chart**  
![](https://raw.githubusercontent.com/cblb-app/cblb-token-model/master/imgs/100-checkin-polygon.png)

**1,000 times check-in token issue chart**  
![](https://raw.githubusercontent.com/cblb-app/cblb-token-model/master/imgs/1000-checkin-polygon.png)

**10,000 times check-in token issue chart**  
![](https://raw.githubusercontent.com/cblb-app/cblb-token-model/master/imgs/10000-checkin-polygon.png)

**100,000 times check-in token issue chart**  
![](https://raw.githubusercontent.com/cblb-app/cblb-token-model/master/imgs/100000-checkin-polygon.png)
