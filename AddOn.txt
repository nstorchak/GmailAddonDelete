function AddOn(event) {

  //create the action and pass the callback function name
  var deleteEmailAction = CardService.newAction()
    .setFunctionName("deleteThatEmail");

  //create a button and register the action it needs to call
  var deleteButton = CardService.newTextButton()
    .setText('Move To Trash')
    .setOnClickAction(deleteEmailAction);

  //create a card  
  var card = CardService.newCardBuilder();
  card.setHeader(CardService.newCardHeader().setTitle(" "));

  //create a section
  var section = CardService.newCardSection();

  //add the button to the section
  section.addWidget(CardService.newButtonSet()
    .addButton(deleteButton));

  //add the section to the button
  card.addSection(section);

  //return the built card
  return [card.build()];

}