# SmartContracts
#### RetransGraph is  a large-scale graph dataset of reentrancy vulnerability in compile-passed smart contract, which is built from 70,904 open-source contracts and labeled with transaction sequences by a NLP labeling schema, BIOES. 

#### Related to our Paper. Updating




The parted AST of 0x0a00b643a01488cc24ed92cbff0fc7de15fe7707.sol is shown as follows:
 ```python
 "sources": {
    "reentrancy": {
      "ast": {
        "absolutePath": "reentrancy",
        "exportedSymbols": {
          "DolaCore": [
            263
          ],
          "LibBytes": [
            747
          ],
          "LibSignatureValidation": [
            61
          ],
          "LibTransferRequest": [
            164
          ]
        },
        "id": 748,
        "nodeType": "SourceUnit",
        "nodes": [
          {
            "id": 1,
            "literals": [
              "solidity",
              "^",
              "0.4",
              ".25"
            ],
            "nodeType": "PragmaDirective",
            "src": "71:24:0"
          },
          {
            "id": 2,
            "literals": [
              "experimental",
              "ABIEncoderV2"
            ],
            "nodeType": "PragmaDirective",
            "src": "97:33:0"
          },
          {
            "baseContracts": [],
            "contractDependencies": [],
            "contractKind": "contract",
            "documentation": null,
            "fullyImplemented": true,
            "id": 61,
            "linearizedBaseContracts": [
              61
            ],
            "name": "LibSignatureValidation",
            "nodeType": "ContractDefinition",
            "nodes": [
              {
                "id": 5,
                "libraryName": {
                  "contractScope": null,
                  "id": 3,
                  "name": "LibBytes",
                  "nodeType": "UserDefinedTypeName",
                  "referencedDeclaration": 747,
                  "src": "179:8:0",
                  "typeDescriptions": {
                    "typeIdentifier": "t_contract$_LibBytes_$747",
                    "typeString": "library LibBytes"
                  }
                },
                "nodeType": "UsingForDirective",
                "src": "173:25:0",
                "typeName": {
                  "id": 4,
                  "name": "bytes",
                  "nodeType": "ElementaryTypeName",
                  "src": "192:5:0",
                  "typeDescriptions": {
                    "typeIdentifier": "t_bytes_storage_ptr",
                    "typeString": "bytes"
                  }
                }
              },
              {
                "body": {
                  "id": 59,
                  "nodeType": "Block",
                  "src": "320:281:0",
                  "statements": [
                    {
                      "expression": {
                        "argumentTypes": null,
                        "arguments": [
                          {
                            "argumentTypes": null,
                            "commonType": {
                              "typeIdentifier": "t_uint256",
                              "typeString": "uint256"
                            },
                            "id": 20,
                            "isConstant": false,
                            "isLValue": false,
                            "isPure": false,
                            "lValueRequested": false,
                            "leftExpression": {
                              "argumentTypes": null,
                              "expression": {
                                "argumentTypes": null,
                                "id": 17,
                                "name": "signature",
                                "nodeType": "Identifier",
                                "overloadedDeclarations": [],
                                "referencedDeclaration": 11,
                                "src": "335:9:0",
                                "typeDescriptions": {
                                  "typeIdentifier": "t_bytes_memory_ptr",
                                  "typeString": "bytes memory"
                                }
                              },
                              "id": 18,
                              "isConstant": false,
                              "isLValue": false,
                              "isPure": false,
                              "lValueRequested": false,
                              "memberName": "length",
                              "nodeType": "MemberAccess",
                              "referencedDeclaration": null,
                              "src": "335:16:0",
                              "typeDescriptions": {
                                "typeIdentifier": "t_uint256",
                                "typeString": "uint256"
                              }
                            },
                            "nodeType": "BinaryOperation",
                            "operator": "==",
                            "rightExpression": {
                              "argumentTypes": null,
                              "hexValue": "3635",
                              "id": 19,
                              "isConstant": false,
                              "isLValue": false,
                              "isPure": true,
                              "kind": "number",
                              "lValueRequested": false,
                              "nodeType": "Literal",
                              "src": "355:2:0",
                              "subdenomination": null,
                              "typeDescriptions": {
                                "typeIdentifier": "t_rational_65_by_1",
                                "typeString": "int_const 65"
                              },
                              "value": "65"
                            },
                            "src": "335:22:0",
                            "typeDescriptions": {
                              "typeIdentifier": "t_bool",
                              "typeString": "bool"
                            }
                          },
                          {
                            "argumentTypes": null,
                            "hexValue": "4c454e4754485f36355f5245515549524544",
                            "id": 21,
                            "isConstant": false,
                            "isLValue": false,
                            "isPure": true,
                            "kind": "string",
                            "lValueRequested": false,
                            "nodeType": "Literal",
                            "src": "359:20:0",
                            "subdenomination": null,
                            "typeDescriptions": {
                              "typeIdentifier": "t_stringliteral_024a7a66bc4464a7341baebd243328b46def44f6001996c320f7f7ea41913014",
                              "typeString": "literal_string \"LENGTH_65_REQUIRED\""
                            },
                            "value": "LENGTH_65_REQUIRED"
                          }
                        ],
                        "expression": {
                          "argumentTypes": [
                            {
                              "typeIdentifier": "t_bool",
                              "typeString": "bool"
                            },
                            {
                              "typeIdentifier": "t_stringliteral_024a7a66bc4464a7341baebd243328b46def44f6001996c320f7f7ea41913014",
                              "typeString": "literal_string \"LENGTH_65_REQUIRED\""
                            }
                          ],
                          "id": 16,
                          "name": "require",
                          "nodeType": "Identifier",
                          "overloadedDeclarations": [
                            765,
                            766
                          ],
                          "referencedDeclaration": 766,
                          "src": "327:7:0",
                          "typeDescriptions": {
                            "typeIdentifier": "t_function_require_pure$_t_bool_$_t_string_memory_ptr_$returns$__$",
                            "typeString": "function (bool,string memory) pure"
                          }
                        },
                        "id": 22,
                        "isConstant": false,
                        "isLValue": false,
                        "isPure": false,
                        "kind": "functionCall",
                        "lValueRequested": false,
                        "names": [],
                        "nodeType": "FunctionCall",
                        "src": "327:53:0",
                        "typeDescriptions": {
                          "typeIdentifier": "t_tuple$__$",
                          "typeString": "tuple()"
                        }
                      },
 ```

 ```python
JSON File: 0x00a03e1dc6ccb4de2ac005c93ce20ac009baba96.json
Node 21,FunctionDefinition,transferFrom [0.041961886 -0.1254507 -0.47043517 0.1314179 0.215371 -0.080254 0.53894407 0.4485073 0.42258543 -0.093240164 -0.31973532 0.44890943 0.026989162 0.20354697 -0.8416363 -0.41461918]
Node 12,VariableDeclaration,from [-0.07370265 0.12989286 -0.40624 -0.1036957 0.21024781 -0.008587352 0.6058331 0.30817726 0.3952153 -0.060758222 -0.006407448 0.2019628 -0.14899899 0.17547214 -0.6901315 -0.49410325]
Node 14,VariableDeclaration,to [0.03505404 0.20624904 -0.14887977 -0.37412825 0.29601598 -0.07769163 0.5464013 0.29321578 0.53010243 0.07235895 0.18125355 0.46226904 0.021504167 -0.11977424 -0.8894709 -0.23234208]
Node 16,VariableDeclaration,value [-0.16719916 -0.045936454 -0.21270123 0.1050977 -0.12351296 0.022303116 0.72627395 0.20824699 0.45337993 -0.16679789 -0.0966535 0.46623215 -0.10557619 -0.009725432 -0.6742142 -0.39413023]
Node 19,VariableDeclaration,constructor [-0.020121979 0.17525655 -0.35311845 0.087004974 0.1437112 0.049789008 0.6402762 0.16230692 0.3666953 -0.15259407 -0.09582282 0.32209882 -0.14244106 0.030734893 -0.67833745 -0.34870335]
Node 66,FunctionDefinition,disperseTokenSimple [-0.044564117 0.14921224 -0.27801725 0.025279125 0.20808743 0.019178262 0.60901195 0.32349116 0.2829351 -0.1599084 0.006705193 0.17929965 0.11082308 -0.034866013 -0.7514331 -0.44357297]
Node 64,ForStatement,IfStatement [-0.02869569 0.15258555 -0.2852772 0.080742404 0.10386761 -0.05710049 0.66562295 0.25933576 0.296117 -0.0961441 -0.037048038 0.2680959 -0.08416226 0.15182498 -0.71156174 -0.36496082]
Node 50,MemberAccess,sender [0.085969456 0.4105578 -0.35468408 0.34998655 -0.044593986 0.029967466 0.6667711 -0.0012820838 0.26137286 -0.30439383 -0.09952816 0.33453485 -0.069355205 0.11935551 -0.56595457 -0.35319608]
Node 48,MemberAccess,None [0.16797955 0.16115773 -0.26140633 -0.003145024 0.28150642 -0.078775026 0.6785409 0.020398147 0.15625224 -0.054400913 -0.06755104 0.1726438 -0.09365967 0.031969488 -0.90059423 -0.06489688]
Node 41,MemberAccess,length [-0.426281 0.40588543 -0.17973953 0.089418896 0.39899567 0.10418487 0.6760778 -0.25733212 0.23416771 0.3297585 -0.36941922 -0.12715568 0.04744896 0.091758415 -0.42552143 -0.32272974]
Node 36,VariableDeclaration,i [-0.35809729 0.23924354 0.068224065 -0.08202927 -0.060230125 0.20797482 0.8621823 -0.35560992 0.29692152 0.05940006 -0.08822442 -0.2240601 0.31704298 -0.005267585 -0.58928925 -0.13116522]
Node 24,VariableDeclaration,token [-0.3101062 0.5185929 0.113098934 0.05946798 0.053580336 0.09250236 0.90116364 -0.5199832 0.14053573 0.1750554 -0.19056955 0.23366725 0.24802305 0.25405625 -0.40871736 0.038275767]
Node 28,VariableDeclaration,recipients [-0.32573587 0.6068019 -0.036397032 0.32301718 0.36962038 0.3419763 0.63412386 -0.3690071 0.20644851 -0.033546858 0.049760208 -0.44532716 0.2787577 0.08004643 -0.63543594 -0.03225654]
Node 32,VariableDeclaration,values [-0.38248533 0.43757612 0.051417056 0.24112342 0.08886392 0.23955733 0.977581 -0.3988751 0.19650935 0.30080587 -0.16026753 -0.14000142 0.38126323 0.12183322 -0.35672343 -0.078687415]
Edge 21 12 [-0.003092702 -0.01629515 0.19110958 -0.0136274705 0.04528128 0.0006891694 0.32651016 0.13821976 0.16701223 0.0056651067 0.0020486875 0.09066301 -0.0040213577 0.035716824 0.5808397 0.20486468]
Edge 12 14 [-0.0025835754 0.026790278 0.060480915 0.03879549 0.06223671 0.0006671654 0.331028 0.09036244 0.20950459 -0.0043964013 -0.0011613728 0.09336115 -0.0032040991 -0.021017041 0.61385185 0.114800975]
Edge 14 16 [-0.005861006 -0.00947435 0.03166691 -0.039320022 -0.03656181 -0.0017327653 0.39683706 0.061061304 0.2403378 -0.01206932 -0.01751879 0.21552469 -0.002270328 0.0011648561 0.5996939 0.09157304]
Edge 16 19 [0.0033643781 -0.008050664 0.07510873 0.009144023 -0.017750194 0.00111045 0.46501592 0.033799928 0.1662523 0.02545237 0.009261611 0.15017283 0.015038384 -0.0002989101 0.45734474 0.13743453]
Edge 19 19 [0.00040489403 0.030714858 0.12469264 0.007569866 0.020652907 0.0024789453 0.4099536 0.026343536 0.13446546 0.023284951 0.009182013 0.10374765 0.020289456 0.0009446336 0.4601417 0.12159403]
Edge 19 66 [0.0008967182 0.026150422 0.09817302 0.0021994095 0.029904492 0.00095486664 0.38993585 0.052504852 0.10375098 0.024401074 -0.0006425105 0.057752207 -0.015785757 -0.0010716032 0.5097252 0.15467538]
Edge 66 64 [0.0012787981 0.022767631 0.07931198 0.0020410973 0.021613544 -0.0010950882 0.40537232 0.08389282 0.0837819 0.01537425 -0.00024841423 0.048069503 -0.00932712 -0.005293532 0.53469104 0.16188675]
Edge 64 64 [0.0008234426 0.023282351 0.08138307 0.006519336 0.010788481 0.003260466 0.4430539 0.067255035 0.08768528 0.009243689 0.0013725571 0.071875416 0.0070832856 0.023050824 0.5063201 0.1331964]
Edge 64 50 [-0.002466953 0.06264519 0.10118328 0.028258756 -0.004631871 -0.001711157 0.44381815 -0.00033249016 0.07739695 0.029265672 0.0036873233 0.08968743 0.005837091 0.018121148 0.40271163 0.12890273]
Edge 50 48 [0.014441111 0.06616456 0.092716664 -0.0011007161 -0.0125534935 -0.0023606878 0.45243147 -2.6152135e-05 0.040840093 0.016559303 0.0067232307 0.057755366 0.0064957854 0.0038157345 0.5096954 0.022921324]
Edge 48 21 [0.0070487387 -0.02021735 0.12297473 -0.00041331243 0.060628317 0.0063220114 0.3656956 0.009148718 0.06602992 0.00507235 0.021598453 0.07750143 -0.002527796 0.0065072924 0.7579728 0.026907492]
Edge 48 41 [-0.071606494 0.065411575 0.046985053 -0.00028122458 0.11231984 -0.008207166 0.4587464 -0.0052490984 0.036589228 -0.017939163 0.024954652 -0.021952638 -0.004444054 0.0029334696 0.38322216 0.020944154]
Edge 41 36 [0.15265007 0.097105466 -0.012262561 -0.0073349667 -0.024031559 0.02166783 0.5829023 0.09150986 0.06952943 0.019587673 0.032591797 0.028490514 0.015043359 -0.00048334527 0.2507552 0.042330917]
Edge 36 24 [0.111048184 0.124069996 0.007716069 -0.004878115 -0.0032271503 0.019238163 0.77696735 0.18491118 0.041728083 0.010398301 0.016812887 -0.05235551 0.078633964 -0.0013382629 0.24085274 -0.0050204494]
Edge 24 28 [0.10101271 0.31468317 -0.004116466 0.019209178 0.019804385 0.031633615 0.57144934 0.19187748 0.029013392 -0.0058725583 -0.0094827805 -0.10405838 0.06913833 0.020336296 0.2597137 -0.0012346439]
Edge 28 32 [0.12458919 0.26552203 -0.0018714282 0.077887006 0.032845914 0.08192293 0.61990744 0.14718774 0.040569063 -0.0100910915 -0.007974946 0.062346432 0.10628006 0.009752315 0.22667488 0.0025381837]
 ```
