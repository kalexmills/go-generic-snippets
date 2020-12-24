# Go2Go Snippets

To better understand the impact of the Go generics proposal, this repository collects a list of solutions to problems that could benefit from generics and links to implementations that run on the [go2go Playground](https://go2goplay.golang.org/p/rC4sofqXuA5). Multiple implementations for the same problem are highly encouraged. Having a variety of solutions to look at and compare will help the community learn about idioms that may be useful.

If you are copying from an online source, please make sure 1) you are able to do so and 2) include a link back to the original material.

Pull requests are welcome, both for examples of the problems shown here and for new ones! Just include a `main` method to demonstrate correct usage. Maintainers reserve the right to run format on your go2go example and change the link, but we will preserve your original commit in the history.

If you see an implementation in this list that you have questions about or want to discuss, start a conversation in the issue tracker.

### Data structures

#### Queue
FIFO access to a list.

* enqueue and dequeue (standard example) ([go2go](https://go2goplay.golang.org/p/WU9wGGNraGB))

#### Graph
Data structure consisting of nodes and edges.

### Algorithms

#### Min / Max
Find smallest/largest element in slice.

* using a numeric interface ([go2go](https://go2goplay.golang.org/p/-SpQWxkaubc))

#### Average / Standard Deviation
Find average/standard deviation of slice.

#### Reverse
Reverse a list

* example from 'Why Generics' ([go2go](https://go2goplay.golang.org/p/birTLemLU3l)) ([source](https://blog.golang.org/why-generics))

#### Union / Intersection
Compute union/intersection of maps.

* using 'sets' -- maps with empty structs for values ([go2go](https://go2goplay.golang.org/p/8D4zmkrUkkK))

#### Shortest Path
Find shortest path in node/edge graphs.

#### `map` over Collections
Apply an arbitrary transformation function to slice/map, returning new slice/map.

* mapping over slices ([go2go](https://go2goplay.golang.org/p/5fxKKfXYCMK))

#### Channel timeout
Read from a channel with a timeout.

#### Join channels
Combine two channels into a single channel.

#### Parallel `map`
Call a list of functions in parallel, returning a slice of results.

#### Parallel `oneOf` 
Call a list of functions using a Context, return the result of the first function to finish, while canceling and cleaning up extra goroutines.
