# TITTLE
F(A,B,C,D) =   ∑m(0,2,8,10,12,13,14,15)+∑d(5,7)   Simplify and implement using verilog                                                      

# THEORY

THE KMAP
The K-map method is particularly useful for reducing complex logic functions, especially those with
multiple variables, into a simplified form. By grouping adjacent cells that have the value of 1,
known as minterms, patterns and common terms can be identified. These groupings can then be
used to derive a simplified Boolean expression that requires fewer logic gates to implement.

The Karnaugh map follows specific rules for grouping cells: the groups must be rectangular in
shape and their sizes must be powers of 2 (1, 2, 4, 8, etc.). Each group should encompass as many
minterms as possible, while still being adjacent in the grid. By combining these groups, redundant
terms can be eliminated, resulting in a minimized expression.

Using the K-map method helps to reduce the complexity and size of logic circuits, which in turn
can lead to improved performance, reduced power consumption, and easier circuit design. It is a
visual and intuitive technique that simplifies the process of logic minimization, allowing designers
to optimize digital systems efficiently. The Karnaugh map is widely used in fields such as computer
engineering, digital electronics, and computer science to achieve optimal logic circuit design.

# LOGIC DIAGRAM
![Screenshot 2023-06-22 133917](https://github.com/jeyaqbalan7/Simulation-project--Digital-Electronics/assets/119393851/e8499f5a-190b-4d54-927a-6406c75671a4)

# NETLIST DIAGRAM
![Screenshot 2023-06-22 133917](https://github.com/jeyaqbalan7/Simulation-project--Digital-Electronics/assets/119393851/e8499f5a-190b-4d54-927a-6406c75671a4)

# TIMING DIAGRAM
![Screenshot 2023-06-22 134203](https://github.com/jeyaqbalan7/Simulation-project--Digital-Electronics/assets/119393851/54c05fd8-f96a-476e-b6c6-0ccf486c19e0)

# PROGRAM
```
module jeua(a,b,c,d,f);
input a,b,c,d;
output f;
wire p,q,bdash,ddash;
not(bdash,b);
not(ddash,d);
and(p,a,b);
and(q,bdash,ddash);
or(f,p,q);
endmodule
```

### SIMPLIFICATION
![image](https://github.com/jeyaqbalan7/Simulation-project--Digital-Electronics/assets/119393851/22712460-ce52-4d30-8ca6-1c9421020048)

