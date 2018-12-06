//callback function for AddOn.gs file
function deleteThatEmail(e) {
  //get current message id
  var accessToken = e.messageMetadata.accessToken;
  var messageId = e.messageMetadata.messageId;
  GmailApp.setCurrentMessageAccessToken(accessToken);
  var message = GmailApp.getMessageById(messageId)

  //move current message to Trash
  GmailApp.moveMessageToTrash(message);
}
