
# Levenshtein-Transitions

Two jQuery functions:

* levenshteinTransition
* levenshteinTransitions

## levenshteinTransition

Transition a jQuery collection from its initial texts, to a target piece of text.

### Options

* minimumWait
* maximumWaitOffset
* targetPhrase
* callback

### Example

		$('.transition').levenshteinTransition(
				{targetPhrase: "New-Phrase"})

## levenshteinTransitions

Transition a jQuery collection from its initial texts, through a list of texts,
then loop back to the start.

### Options

* delay
* initialDelay
* targetPhrases
* includeInitialText

Also passes through all of the options for levenshteinTransition, except
targetPhrase and callback.

### Example

		$('.transitions').levenshteinTransitions(
				{delay: 1000, targetPhrases: ["New-Phrase 1", "New-Phrase 2"]})
