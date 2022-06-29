############### SCRABBLE GAME ################

letters = ["A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z", " "]
points = [1, 3, 3, 2, 1, 4, 2, 4, 1, 8, 5, 1, 3, 4, 1, 3, 10, 1, 1, 1, 1, 4, 4, 8, 4, 10, 0]


###Creating dictionary, key:value letter:points
letter_to_points = {key:value for key, value in zip(letters, points)}
#print(letter_to_points)


###Function for calculating the score of a word
def score_word(word):
  point_total = 0
###Points' counter
  for letter in word:
###Accessing letter's value and adding it to the counter
    point_total += letter_to_points.get(letter, 0)
  return point_total


###Testing score_word() with a single word
brownie_points = score_word("BROWNIE")
#print("\"BROWNIE\" Points:", brownie_points, "\n\n")


############### MULTIPLAYER GAME ################

###Dictionary of players and their words
player_to_words = {"Nadia": ["BLUE", "SUN", "ROSE"], "Brett": ["SLOTH", "EYES", "LOVE"], "Ana": ["CLOUD", "CHERRY", "DOG"], "Ale": ["YOGURT", "ICE", "HUSKY"]}

print("PLAYERS' NAMES AND WORDS: \n")


###Adding one more player to dictionary player_to_words{}
def play_word(player, word):
  player_to_words[player] = word

added_play_word = play_word("Juan", ["TEQUILA", "SHOT", "PLEASE"])


###Displaying player's name, player's number and their words
player = 0
for key, value in player_to_words.items():
  player+=1 ###Player number, key:value name:listofwords
  print("Player {}: ".format(player) + key + "\nWords: " + str(value), "\n")

print("\n\nSCORES: \n")


###Counting points- Final Score
player = 0
for key, value in player_to_words.items():
  player_points = 0
  player+=1
  player_to_points= {}
  for word in value:
###Counting points in each word, calling score_word function
    player_points += score_word(word)
###Dictionary with key:value, playername:score
    player_to_points[key] = player_points
##Displaying player number and their score
  print("Player {} points: ".format(player) + str(player_points))
###Displaying dictionary style player_to_points playername:score
  print(player_to_points, "\n") 









