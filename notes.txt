# RNCourse
 Practice React Native
 An App to Track Goals
    Add remove Goals
 node.js
 expo - cli

 Run `npm install` to install all dependencies for the project
 `npm start` to start application

 #CSS
 flexbox - turned on by default
 flexDirection , row col reverse etc

 justifyContent: ' '- organize elements along main axis
 alignItems: ' ' - organize elements on cross axis

 flex - applied to items inside a flexbox
 flex: 1 - item takes as much space as it can

 #Handle Events like click button

 #states

 if your new state depends on a previous state its best to pass a function(state update function)
 function called automaticaly by react

 Notes:
 Example display array
         <ScrollView>
          {allGoals.map((goal) => (
            <View style={styles.goalItem} key={goal}>
              <Text style={styles.goalText}>{goal}</Text>
            </View>
          ))}
        </ScrollView>

FlatList: keyExtractor={(item, index) => {//called to get a key out of every item
   return item.id;
} }


#ios style prop for Pressable
style={({pressed}) pressed && styles.pressedItem}
