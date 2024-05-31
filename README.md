
# The LAbS language: example specifications 

This repository contains some examples of multi-agent systems specified in the
LAbS language [[1]](#references). They may be analyzed with the
[SLiVER](https://github.com/labs-lang/sliver) tool.

## Description of the examples

### `alpha.labs`

A (tentative) implementation of the alpha-algorithm for swarm aggregation
[[8]](#references).

### `approx-majority.labs`

Implements the *approximate majority* population protocol [[6]](#references).

### `boids-[c?a?s?w?].labs`

These are several variants of the *boids* model of flocking behavior
[[5]](#references).
Agents move in a 2D arena and try to agree on the direction of movement or
on the *leader* of the flock (depending on the variant).

Agents have up to three behavioral rules, called *cohesion*, *alignment*, and
*separation*.
The letters `c`, `a`, `s` in the file name indicate which rules are enabled
for that file.
The letter `w` denotes systems where the arena wraps around (i.e. an agent can
cross the edge of the arena and get to the opposite side).

### `formation.labs`

Agents move on a line of size `_size` and attempt to reach a state where their distance from
each other is at least `_delta`.

### `leader.labs`

A simple leader election over a stigmergy. Nodes repeatedly publish their own
id on a stigmergic variable: the node with the lowest id (namely, 0) eventually
is chosen as leader by all nodes.

### `majority.labs`

Implements a (correct) *majority* population protocol [[7]](#references).

### `philosophers.labs`

A LAbS implementation of the well-known dining philosophers problem.
This example showcases some LAbS features such as arrays and environment
variables (which act as a shared memory).

### `cmsb2023`

A model of pheromone-sensing foraging ants that has been presented at CMSB'23 [[10]](#references).

### `isola2022-scp2023/`

Models that were presented in a paper at ISoLA'22 [[3]](#references)
and its extended version on STTT [[4]](#references).
They include five, increasingly complex, flock-of-birds specifications,
and a recreation of the classic double-bridge ant colony experiment [[9]](#references).

## Support

If you have questions, or find that some specifications don't behave as you would expect,
please submit an [issue](https://github.com/labs-lang/labs-examples/issues).

## References

(Apologies, but references are in no particular order).

[1] R. De Nicola, L. Di Stefano, and O. Inverso, “Multi-Agent Systems with Virtual Stigmergy,” in Software Technologies: Applications and Foundations. STAF 2018. LNCS, vol 11176. Springer, 2018. [Link](https://link.springer.com/chapter/10.1007%2F978-3-030-04771-9_26)

[2] R. De Nicola, L. Di Stefano, and O. Inverso. 2020. Multi-agent systems with virtual stigmergy. Science of Computer Programning 187, 2020. [Link](https://doi.org/10.1016/j.scico.2019.102345)

[3] R. De Nicola, L. Di Stefano, O. Inverso, and S. Valiani, "Modelling Flocks of Birds from the Bottom Up". In 11th International Symposium on Leveraging Applications of Formal Methods, Verification and Validation. Adaptation and Learning (ISoLA). LNCS, vol 13703. Springer, 2022. [Link](https://doi.org/10.1007/978-3-031-19759-8_6)

[4] R. De Nicola, L. Di Stefano, O. Inverso, and S. Valiani, "Modelling flocks of birds and colonies of ants from the bottom up," International Journal of Software Tools for Technology Transfer 25, 2023. [Link](https://doi.org/10.1007/s10009-023-00731-0)

[5] C. W. Reynolds, “Flocks, herds and schools: A distributed behavioral model,” in 14th Annual Conference on Computer Graphics and Interactive Techniques (SIGGRAPH), Anaheim, CA, USA, 1987, vol. 21, pp. 25–34.

[6] D. Angluin, J. Aspnes, and D. Eisenstat, “A simple population protocol for fast robust approximate majority,” Distributed Computing, vol. 21, no. 2, pp. 87–102, 2008.

[7] J. Aspnes and E. Ruppert, “An Introduction to Population Protocols,” in Middleware for Network Eccentric and Mobile Applications, B. Garbinato, H. Miranda, and L. E. T. Rodrigues, Eds. Springer, 2009, pp. 97–120.

[8] A. F. T. Winfield, W. Liu, J. Nembrini, and A. Martinoli, “Modelling a wireless connected swarm of mobile robots,” Swarm Intelligence, vol. 2, no. 2–4, pp. 241–266, 2008, doi: 10.1007/s11721-008-0018-0.

[9] S. Goss, S. Aron, J. L. Deneubourg, and J. M. Pasteels. 1989. Self-organized shortcuts in the Argentine ant. Naturwissenschaften 76, 1989. [Link](https://doi.org/10.1007/BF00462870)

[10] R. De Nicola, L. Di Stefano, O. Inverso, and S. Valiani, "Intuitive Modelling and Formal Analysis of Collective Behaviour in Foraging Ants," in 21st International Conference on Computational Methods in Systems Biology (CMSB). LNCS, vol 14137. Springer, 2023. [Link](https://doi.org/10.1007/978-3-031-42697-1_4)
