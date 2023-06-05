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
