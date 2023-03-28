

# Design for new "Create" elements mechanism








Requirements:<br><ol><li>Only create an orphan node instead of creating the node and the relationship</li><li>Should not involve "Undo"</li><li>Impact offline and online both.</li><li>New element should be created whether it is an orphan node or it is already be associated</li></ol><br><br>Blocking defects fixing of:<br>[DEF]Service view: Implementation is applied after clicking cancel button #2816<br>[DEF]Error '' pops up when adding a new DU for LN #3325<br>[DEF]Show a new DU '[No Label]' in the DU list when go back to LN's info page #3512<br>[DEF]Add DU under LN, but do not associate LN and PN .DU should not be included in PN directly&nbsp; #3675<br>

