# DJ-Playlist

Description: The propose of this Lab, was to create a playlist for a DJ using a data structure binary search tree. The playlist contains, the song name, artist, average number of plays for each song, and the average number of plays for each artist.

Instruction: The way we obtain this information goes as following:

Frist, we create a class called BinarySearchTree that has inner class called song; the song class represents a node that would store the data in the binary search tree. In addtion, the song class would count the average number of plays for each song as well as the average number of plays for each artist. However, to get the proper averages, we need to consider the different serineros that might occur. For instance, to get the average of the song title of every song that’s being added to the binary search tree, if it has the same song title, we sum up the total number plays and divide with number of time its repeated. If the song title is not repeated, then the average number of plays is equal to the number of plays. Same situation goes for the average number of artists. Therefore, when returning the data when consider the different serineros; if the song is repeated then we return the data with the average of the song titles else we return the average of the song titles is equal to the plays of that song. We then add the methods to the BinarySearchTree.
The BinarySearchTree will have the following method: insert, subset, and PreOrder. The insert method adds the song node of each song to the binary search trees by the properties of binary search tree that each parent has two children, the smaller vlaues goes to the left and the larger values goes to the right. It also calls the methods the methods averageStreamCount which calculates the average song title plays and the method avgArtist which calculates the average artist plays. The Subset method controls the range in which you want to retrieve the data from song to another. The PreOrder method prints the data in in Order traversal, which is (left, root, right).

Second, we create a DjPlaylist class that retives the data from muitple csv files and instantiate BinarySearchTree object of the BinarySearchTree class and add the data into the BinarySearchTree. The DjPlaylist class has the methods: readFile, storeData, SongList, and print. The readFile method reads all the csv files and stores the data into an Arraylist called storeData. Then will use the storeData method to split the different data into three different arrayLists Songlist, ArtistName, and Streams. Once we have sprarate data we can now insert into the binary search tree using the SongList method. After we are done we can print the data into two separate text files using the print method. One of text file is for the full list containing all the information of the playlist called DjPlayList.txt. The second text file SubSet.txt is for the range of data given the domain of the song titles.
