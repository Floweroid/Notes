# Computer Organization & Programming Systems

> Note for `CIS.341`.`M001`.`FALL23`.`Cptr Organ and Progrmmng Syst` `14189`.`1241`
>
> Author: `Zekai Lin`
>
> Resently Update: `Oct.4 23` `16:18`

``` graphviz

digraph G {

    rankdir=LR // Set the orientation to left-to-right

    // Nodes

    // subject name
    CIS341 [label="CIS.341"]

    // C related
    C [label="programming language C"]
    C_Basics [label="C_Basics"]
    C_ptr_arr [label="C_ptr&arr"]
    C_Memory_Management [label="C_Memory_Management"]

    // data_representation
    data_representation [label="data_representation"]
    Bits_bytes [label="Bits&bytes"]
    Integer [label="Integer"]
    float [label="float"]

    //
    Machine [label="Machine"]
    Machine_organization [label="Machine_organization"]
    Instruction_control_flow_1 [label="Instruction-control_flow_1"]
    Instruction_control_flow_2 [label="Instruction-control_flow_2"]
    Procedures [label="Procedures"]

    // CIS 341
    CIS341 -> C
    CIS341 -> data_representation
    CIS341 -> Machine

    // C 
    C -> C_Basics
    C -> C_ptr_arr
    C -> C_Memory_Management


    // data_representation
    data_representation -> Bits_bytes
    data_representation -> Integer
    data_representation -> float

    // Machine
    Machine -> Machine_organization
    Machine -> Instruction_control_flow_1
    Machine -> Instruction_control_flow_2
    Machine -> Procedures
}

```

## Outline

- [Syllabus](../../res/cis341Fa23Syllabus.pdf)  
- [Lec01-C_Basics](../../nodes/001/index.md)
- [Lec02-C_ptr&arr](../../nodes/002/index.md)
- [Lec03-C_Memory Management](../../nodes/003/index.md)
- [Lec04-Bits & Ints](../../nodes/004/index.md)
- [Lec05-Floats](../../nodes/006/index.md)
