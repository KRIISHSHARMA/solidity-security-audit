ramanujan@ramanujan-HLBS-CM-44:~$ surya parse data.sol 
├─ type: SourceUnit
└─ children
   ├─ 0
   │  ├─ type: PragmaDirective
   │  ├─ name: solidity
   │  └─ value: >=0.8.6 <0.9.0
   ├─ 1
   │  ├─ type: ContractDefinition
   │  ├─ name: contract_example
   │  ├─ baseContracts
   │  ├─ subNodes
   │  │  ├─ 0
   │  │  │  ├─ type: StateVariableDeclaration
   │  │  │  ├─ variables
   │  │  │  │  └─ 0
   │  │  │  │     ├─ type: VariableDeclaration
   │  │  │  │     ├─ typeName
   │  │  │  │     │  ├─ type: ElementaryTypeName
   │  │  │  │     │  ├─ name: uint
   │  │  │  │     │  └─ stateMutability
   │  │  │  │     ├─ name: num1
   │  │  │  │     ├─ identifier
   │  │  │  │     │  ├─ type: Identifier
   │  │  │  │     │  └─ name: num1
   │  │  │  │     ├─ expression
   │  │  │  │     ├─ visibility: private
   │  │  │  │     ├─ isStateVar: true
   │  │  │  │     ├─ isDeclaredConst: false
   │  │  │  │     ├─ isIndexed: false
   │  │  │  │     ├─ isImmutable: false
   │  │  │  │     ├─ override
   │  │  │  │     └─ storageLocation
   │  │  │  └─ initialValue
   │  │  ├─ 1
   │  │  │  ├─ type: StateVariableDeclaration
   │  │  │  ├─ variables
   │  │  │  │  └─ 0
   │  │  │  │     ├─ type: VariableDeclaration
   │  │  │  │     ├─ typeName
   │  │  │  │     │  ├─ type: ElementaryTypeName
   │  │  │  │     │  ├─ name: uint
   │  │  │  │     │  └─ stateMutability
   │  │  │  │     ├─ name: num2
   │  │  │  │     ├─ identifier
   │  │  │  │     │  ├─ type: Identifier
   │  │  │  │     │  └─ name: num2
   │  │  │  │     ├─ expression
   │  │  │  │     ├─ visibility: public
   │  │  │  │     ├─ isStateVar: true
   │  │  │  │     ├─ isDeclaredConst: false
   │  │  │  │     ├─ isIndexed: false
   │  │  │  │     ├─ isImmutable: false
   │  │  │  │     ├─ override
   │  │  │  │     └─ storageLocation
   │  │  │  └─ initialValue
   │  │  ├─ 2
   │  │  │  ├─ type: StateVariableDeclaration
   │  │  │  ├─ variables
   │  │  │  │  └─ 0
   │  │  │  │     ├─ type: VariableDeclaration
   │  │  │  │     ├─ typeName
   │  │  │  │     │  ├─ type: ElementaryTypeName
   │  │  │  │     │  ├─ name: string
   │  │  │  │     │  └─ stateMutability
   │  │  │  │     ├─ name: str
   │  │  │  │     ├─ identifier
   │  │  │  │     │  ├─ type: Identifier
   │  │  │  │     │  └─ name: str
   │  │  │  │     ├─ expression
   │  │  │  │     ├─ visibility: internal
   │  │  │  │     ├─ isStateVar: true
   │  │  │  │     ├─ isDeclaredConst: false
   │  │  │  │     ├─ isIndexed: false
   │  │  │  │     ├─ isImmutable: false
   │  │  │  │     ├─ override
   │  │  │  │     └─ storageLocation
   │  │  │  └─ initialValue
   │  │  ├─ 3
   │  │  │  ├─ type: FunctionDefinition
   │  │  │  ├─ name
   │  │  │  ├─ parameters
   │  │  │  ├─ returnParameters
   │  │  │  ├─ body
   │  │  │  │  ├─ type: Block
   │  │  │  │  └─ statements
   │  │  │  │     └─ 0
   │  │  │  │        ├─ type: ExpressionStatement
   │  │  │  │        └─ expression
   │  │  │  │           ├─ type: BinaryOperation
   │  │  │  │           ├─ operator: =
   │  │  │  │           ├─ left
   │  │  │  │           │  ├─ type: Identifier
   │  │  │  │           │  └─ name: num2
   │  │  │  │           └─ right
   │  │  │  │              ├─ type: NumberLiteral
   │  │  │  │              ├─ number: 10
   │  │  │  │              └─ subdenomination
   │  │  │  ├─ visibility: default
   │  │  │  ├─ modifiers
   │  │  │  ├─ override
   │  │  │  ├─ isConstructor: true
   │  │  │  ├─ isReceiveEther: false
   │  │  │  ├─ isFallback: false
   │  │  │  ├─ isVirtual: false
   │  │  │  └─ stateMutability
   │  │  ├─ 4
   │  │  │  ├─ type: FunctionDefinition
   │  │  │  ├─ name: increment
   │  │  │  ├─ parameters
   │  │  │  │  └─ 0
   │  │  │  │     ├─ type: VariableDeclaration
   │  │  │  │     ├─ typeName
   │  │  │  │     │  ├─ type: ElementaryTypeName
   │  │  │  │     │  ├─ name: uint
   │  │  │  │     │  └─ stateMutability
   │  │  │  │     ├─ name: data1
   │  │  │  │     ├─ identifier
   │  │  │  │     │  ├─ type: Identifier
   │  │  │  │     │  └─ name: data1
   │  │  │  │     ├─ storageLocation
   │  │  │  │     ├─ isStateVar: false
   │  │  │  │     ├─ isIndexed: false
   │  │  │  │     └─ expression
   │  │  │  ├─ returnParameters
   │  │  │  │  └─ 0
   │  │  │  │     ├─ type: VariableDeclaration
   │  │  │  │     ├─ typeName
   │  │  │  │     │  ├─ type: ElementaryTypeName
   │  │  │  │     │  ├─ name: uint
   │  │  │  │     │  └─ stateMutability
   │  │  │  │     ├─ name
   │  │  │  │     ├─ identifier
   │  │  │  │     ├─ storageLocation
   │  │  │  │     ├─ isStateVar: false
   │  │  │  │     ├─ isIndexed: false
   │  │  │  │     └─ expression
   │  │  │  ├─ body
   │  │  │  │  ├─ type: Block
   │  │  │  │  └─ statements
   │  │  │  │     └─ 0
   │  │  │  │        ├─ type: ReturnStatement
   │  │  │  │        └─ expression
   │  │  │  │           ├─ type: BinaryOperation
   │  │  │  │           ├─ operator: +
   │  │  │  │           ├─ left
   │  │  │  │           │  ├─ type: Identifier
   │  │  │  │           │  └─ name: data1
   │  │  │  │           └─ right
   │  │  │  │              ├─ type: NumberLiteral
   │  │  │  │              ├─ number: 1
   │  │  │  │              └─ subdenomination
   │  │  │  ├─ visibility: private
   │  │  │  ├─ modifiers
   │  │  │  ├─ override
   │  │  │  ├─ isConstructor: false
   │  │  │  ├─ isReceiveEther: false
   │  │  │  ├─ isFallback: false
   │  │  │  ├─ isVirtual: false
   │  │  │  └─ stateMutability: pure
   │  │  ├─ 5
   │  │  │  ├─ type: FunctionDefinition
   │  │  │  ├─ name: updateValue
   │  │  │  ├─ parameters
   │  │  │  │  └─ 0
   │  │  │  │     ├─ type: VariableDeclaration
   │  │  │  │     ├─ typeName
   │  │  │  │     │  ├─ type: ElementaryTypeName
   │  │  │  │     │  ├─ name: uint
   │  │  │  │     │  └─ stateMutability
   │  │  │  │     ├─ name: data1
   │  │  │  │     ├─ identifier
   │  │  │  │     │  ├─ type: Identifier
   │  │  │  │     │  └─ name: data1
   │  │  │  │     ├─ storageLocation
   │  │  │  │     ├─ isStateVar: false
   │  │  │  │     ├─ isIndexed: false
   │  │  │  │     └─ expression
   │  │  │  ├─ returnParameters
   │  │  │  ├─ body
   │  │  │  │  ├─ type: Block
   │  │  │  │  └─ statements
   │  │  │  │     └─ 0
   │  │  │  │        ├─ type: ExpressionStatement
   │  │  │  │        └─ expression
   │  │  │  │           ├─ type: BinaryOperation
   │  │  │  │           ├─ operator: =
   │  │  │  │           ├─ left
   │  │  │  │           │  ├─ type: Identifier
   │  │  │  │           │  └─ name: num1
   │  │  │  │           └─ right
   │  │  │  │              ├─ type: Identifier
   │  │  │  │              └─ name: data1
   │  │  │  ├─ visibility: public
   │  │  │  ├─ modifiers
   │  │  │  ├─ override
   │  │  │  ├─ isConstructor: false
   │  │  │  ├─ isReceiveEther: false
   │  │  │  ├─ isFallback: false
   │  │  │  ├─ isVirtual: false
   │  │  │  └─ stateMutability
   │  │  ├─ 6
   │  │  │  ├─ type: FunctionDefinition
   │  │  │  ├─ name: getValue
   │  │  │  ├─ parameters
   │  │  │  ├─ returnParameters
   │  │  │  │  └─ 0
   │  │  │  │     ├─ type: VariableDeclaration
   │  │  │  │     ├─ typeName
   │  │  │  │     │  ├─ type: ElementaryTypeName
   │  │  │  │     │  ├─ name: uint
   │  │  │  │     │  └─ stateMutability
   │  │  │  │     ├─ name
   │  │  │  │     ├─ identifier
   │  │  │  │     ├─ storageLocation
   │  │  │  │     ├─ isStateVar: false
   │  │  │  │     ├─ isIndexed: false
   │  │  │  │     └─ expression
   │  │  │  ├─ body
   │  │  │  │  ├─ type: Block
   │  │  │  │  └─ statements
   │  │  │  │     └─ 0
   │  │  │  │        ├─ type: ReturnStatement
   │  │  │  │        └─ expression
   │  │  │  │           ├─ type: Identifier
   │  │  │  │           └─ name: num1
   │  │  │  ├─ visibility: public
   │  │  │  ├─ modifiers
   │  │  │  ├─ override
   │  │  │  ├─ isConstructor: false
   │  │  │  ├─ isReceiveEther: false
   │  │  │  ├─ isFallback: false
   │  │  │  ├─ isVirtual: false
   │  │  │  └─ stateMutability: view
   │  │  ├─ 7
   │  │  │  ├─ type: FunctionDefinition
   │  │  │  ├─ name: setStr
   │  │  │  ├─ parameters
   │  │  │  │  └─ 0
   │  │  │  │     ├─ type: VariableDeclaration
   │  │  │  │     ├─ typeName
   │  │  │  │     │  ├─ type: ElementaryTypeName
   │  │  │  │     │  ├─ name: string
   │  │  │  │     │  └─ stateMutability
   │  │  │  │     ├─ name: _str
   │  │  │  │     ├─ identifier
   │  │  │  │     │  ├─ type: Identifier
   │  │  │  │     │  └─ name: _str
   │  │  │  │     ├─ storageLocation: memory
   │  │  │  │     ├─ isStateVar: false
   │  │  │  │     ├─ isIndexed: false
   │  │  │  │     └─ expression
   │  │  │  ├─ returnParameters
   │  │  │  ├─ body
   │  │  │  ├─ visibility: public
   │  │  │  ├─ modifiers
   │  │  │  ├─ override
   │  │  │  ├─ isConstructor: false
   │  │  │  ├─ isReceiveEther: false
   │  │  │  ├─ isFallback: false
   │  │  │  ├─ isVirtual: true
   │  │  │  └─ stateMutability
   │  │  └─ 8
   │  │     ├─ type: FunctionDefinition
   │  │     ├─ name: getStr
   │  │     ├─ parameters
   │  │     ├─ returnParameters
   │  │     │  └─ 0
   │  │     │     ├─ type: VariableDeclaration
   │  │     │     ├─ typeName
   │  │     │     │  ├─ type: ElementaryTypeName
   │  │     │     │  ├─ name: string
   │  │     │     │  └─ stateMutability
   │  │     │     ├─ name
   │  │     │     ├─ identifier
   │  │     │     ├─ storageLocation: memory
   │  │     │     ├─ isStateVar: false
   │  │     │     ├─ isIndexed: false
   │  │     │     └─ expression
   │  │     ├─ body
   │  │     ├─ visibility: public
   │  │     ├─ modifiers
   │  │     ├─ override
   │  │     ├─ isConstructor: false
   │  │     ├─ isReceiveEther: false
   │  │     ├─ isFallback: false
   │  │     ├─ isVirtual: true
   │  │     └─ stateMutability
   │  └─ kind: abstract
   ├─ 2
   │  ├─ type: ContractDefinition
   │  ├─ name: derived_contract
   │  ├─ baseContracts
   │  │  └─ 0
   │  │     ├─ type: InheritanceSpecifier
   │  │     ├─ baseName
   │  │     │  ├─ type: UserDefinedTypeName
   │  │     │  └─ namePath: contract_example
   │  │     └─ arguments
   │  ├─ subNodes
   │  │  ├─ 0
   │  │  │  ├─ type: FunctionDefinition
   │  │  │  ├─ name: setStr
   │  │  │  ├─ parameters
   │  │  │  │  └─ 0
   │  │  │  │     ├─ type: VariableDeclaration
   │  │  │  │     ├─ typeName
   │  │  │  │     │  ├─ type: ElementaryTypeName
   │  │  │  │     │  ├─ name: string
   │  │  │  │     │  └─ stateMutability
   │  │  │  │     ├─ name: _str
   │  │  │  │     ├─ identifier
   │  │  │  │     │  ├─ type: Identifier
   │  │  │  │     │  └─ name: _str
   │  │  │  │     ├─ storageLocation: memory
   │  │  │  │     ├─ isStateVar: false
   │  │  │  │     ├─ isIndexed: false
   │  │  │  │     └─ expression
   │  │  │  ├─ returnParameters
   │  │  │  ├─ body
   │  │  │  │  ├─ type: Block
   │  │  │  │  └─ statements
   │  │  │  │     └─ 0
   │  │  │  │        ├─ type: ExpressionStatement
   │  │  │  │        └─ expression
   │  │  │  │           ├─ type: BinaryOperation
   │  │  │  │           ├─ operator: =
   │  │  │  │           ├─ left
   │  │  │  │           │  ├─ type: Identifier
   │  │  │  │           │  └─ name: str
   │  │  │  │           └─ right
   │  │  │  │              ├─ type: Identifier
   │  │  │  │              └─ name: _str
   │  │  │  ├─ visibility: public
   │  │  │  ├─ modifiers
   │  │  │  ├─ override
   │  │  │  ├─ isConstructor: false
   │  │  │  ├─ isReceiveEther: false
   │  │  │  ├─ isFallback: false
   │  │  │  ├─ isVirtual: false
   │  │  │  └─ stateMutability
   │  │  └─ 1
   │  │     ├─ type: FunctionDefinition
   │  │     ├─ name: getStr
   │  │     ├─ parameters
   │  │     ├─ returnParameters
   │  │     │  └─ 0
   │  │     │     ├─ type: VariableDeclaration
   │  │     │     ├─ typeName
   │  │     │     │  ├─ type: ElementaryTypeName
   │  │     │     │  ├─ name: string
   │  │     │     │  └─ stateMutability
   │  │     │     ├─ name
   │  │     │     ├─ identifier
   │  │     │     ├─ storageLocation: memory
   │  │     │     ├─ isStateVar: false
   │  │     │     ├─ isIndexed: false
   │  │     │     └─ expression
   │  │     ├─ body
   │  │     │  ├─ type: Block
   │  │     │  └─ statements
   │  │     │     └─ 0
   │  │     │        ├─ type: ReturnStatement
   │  │     │        └─ expression
   │  │     │           ├─ type: Identifier
   │  │     │           └─ name: str
   │  │     ├─ visibility: public
   │  │     ├─ modifiers
   │  │     ├─ override
   │  │     ├─ isConstructor: false
   │  │     ├─ isReceiveEther: false
   │  │     ├─ isFallback: false
   │  │     ├─ isVirtual: false
   │  │     └─ stateMutability: view
   │  └─ kind: contract
   └─ 3
      ├─ type: ContractDefinition
      ├─ name: D
      ├─ baseContracts
      ├─ subNodes
      │  └─ 0
      │     ├─ type: FunctionDefinition
      │     ├─ name: readData
      │     ├─ parameters
      │     ├─ returnParameters
      │     │  ├─ 0
      │     │  │  ├─ type: VariableDeclaration
      │     │  │  ├─ typeName
      │     │  │  │  ├─ type: ElementaryTypeName
      │     │  │  │  ├─ name: string
      │     │  │  │  └─ stateMutability
      │     │  │  ├─ name
      │     │  │  ├─ identifier
      │     │  │  ├─ storageLocation: memory
      │     │  │  ├─ isStateVar: false
      │     │  │  ├─ isIndexed: false
      │     │  │  └─ expression
      │     │  └─ 1
      │     │     ├─ type: VariableDeclaration
      │     │     ├─ typeName
      │     │     │  ├─ type: ElementaryTypeName
      │     │     │  ├─ name: uint
      │     │     │  └─ stateMutability
      │     │     ├─ name
      │     │     ├─ identifier
      │     │     ├─ storageLocation
      │     │     ├─ isStateVar: false
      │     │     ├─ isIndexed: false
      │     │     └─ expression
      │     ├─ body
      │     │  ├─ type: Block
      │     │  └─ statements
      │     │     ├─ 0
      │     │     │  ├─ type: VariableDeclarationStatement
      │     │     │  ├─ variables
      │     │     │  │  └─ 0
      │     │     │  │     ├─ type: VariableDeclaration
      │     │     │  │     ├─ typeName
      │     │     │  │     │  ├─ type: UserDefinedTypeName
      │     │     │  │     │  └─ namePath: contract_example
      │     │     │  │     ├─ name: c
      │     │     │  │     ├─ identifier
      │     │     │  │     │  ├─ type: Identifier
      │     │     │  │     │  └─ name: c
      │     │     │  │     ├─ storageLocation
      │     │     │  │     ├─ isStateVar: false
      │     │     │  │     ├─ isIndexed: false
      │     │     │  │     └─ expression
      │     │     │  └─ initialValue
      │     │     │     ├─ type: FunctionCall
      │     │     │     ├─ expression
      │     │     │     │  ├─ type: NewExpression
      │     │     │     │  └─ typeName
      │     │     │     │     ├─ type: UserDefinedTypeName
      │     │     │     │     └─ namePath: derived_contract
      │     │     │     ├─ arguments
      │     │     │     ├─ names
      │     │     │     └─ identifiers
      │     │     ├─ 1
      │     │     │  ├─ type: ExpressionStatement
      │     │     │  └─ expression
      │     │     │     ├─ type: FunctionCall
      │     │     │     ├─ expression
      │     │     │     │  ├─ type: MemberAccess
      │     │     │     │  ├─ expression
      │     │     │     │  │  ├─ type: Identifier
      │     │     │     │  │  └─ name: c
      │     │     │     │  └─ memberName: setStr
      │     │     │     ├─ arguments
      │     │     │     │  └─ 0
      │     │     │     │     ├─ type: StringLiteral
      │     │     │     │     ├─ value: GeeksForGeeks
      │     │     │     │     ├─ parts
      │     │     │     │     │  └─ 0: GeeksForGeeks
      │     │     │     │     └─ isUnicode
      │     │     │     │        └─ 0: false
      │     │     │     ├─ names
      │     │     │     └─ identifiers
      │     │     ├─ 2
      │     │     │  ├─ type: ExpressionStatement
      │     │     │  └─ expression
      │     │     │     ├─ type: FunctionCall
      │     │     │     ├─ expression
      │     │     │     │  ├─ type: MemberAccess
      │     │     │     │  ├─ expression
      │     │     │     │  │  ├─ type: Identifier
      │     │     │     │  │  └─ name: c
      │     │     │     │  └─ memberName: updateValue
      │     │     │     ├─ arguments
      │     │     │     │  └─ 0
      │     │     │     │     ├─ type: NumberLiteral
      │     │     │     │     ├─ number: 16
      │     │     │     │     └─ subdenomination
      │     │     │     ├─ names
      │     │     │     └─ identifiers
      │     │     └─ 3
      │     │        ├─ type: ReturnStatement
      │     │        └─ expression
      │     │           ├─ type: TupleExpression
      │     │           ├─ components
      │     │           │  ├─ 0
      │     │           │  │  ├─ type: FunctionCall
      │     │           │  │  ├─ expression
      │     │           │  │  │  ├─ type: MemberAccess
      │     │           │  │  │  ├─ expression
      │     │           │  │  │  │  ├─ type: Identifier
      │     │           │  │  │  │  └─ name: c
      │     │           │  │  │  └─ memberName: getStr
      │     │           │  │  ├─ arguments
      │     │           │  │  ├─ names
      │     │           │  │  └─ identifiers
      │     │           │  └─ 1
      │     │           │     ├─ type: FunctionCall
      │     │           │     ├─ expression
      │     │           │     │  ├─ type: MemberAccess
      │     │           │     │  ├─ expression
      │     │           │     │  │  ├─ type: Identifier
      │     │           │     │  │  └─ name: c
      │     │           │     │  └─ memberName: getValue
      │     │           │     ├─ arguments
      │     │           │     ├─ names
      │     │           │     └─ identifiers
      │     │           └─ isArray: false
      │     ├─ visibility: public
      │     ├─ modifiers
      │     ├─ override
      │     ├─ isConstructor: false
      │     ├─ isReceiveEther: false
      │     ├─ isFallback: false
      │     ├─ isVirtual: false
      │     └─ stateMutability
      └─ kind: contract

