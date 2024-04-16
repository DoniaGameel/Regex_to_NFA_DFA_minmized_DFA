# Regex_to_NFA_DFA_minmized_DFA

This tool converts a regular expression into its corresponding Nondeterministic Finite Automaton (NFA) strictly using Thompson’s construction algorithm.

The input to the tool is simply a regular expression in text format. Before transformation, we validate the expression to ensure it is well-formed. An example of an invalid regular expression would be: [A-Za-z

The output is an image displaying the graph of the NFA, utilizing the graphviz library. We visually distinguish between accepting and non-accepting states.

Additionally, we implement a program capable of converting an NFA into a minimized Deterministic Finite Automaton (DFA).

The input for this program is a file containing the JSON representation of the NFA, formatted as follows:

{
  "startingState": "S0",
  "S0": {
    "isTerminatingState": false,
    "A": "S1",
    "B": "S0"
  },
  "S1": {
    "isTerminatingState": true,
    "A": "S1",
    "B": "S1"
  }
}

The output is a JSON file representing the minimized DFA states and transitions, following the same format as the input.

Furthermore, we generate an image illustrating the graph of the minimized DFA using the graphviz library. As with the NFA, we visually distinguish between accepting and non-accepting states.

## Contributors:
[Donia Gameel](https://github.com/DoniaGameel)
[Heba Ashraf](https://github.com/hebaashraf21)
