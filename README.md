A04Q22
======
void swap(struct node *head)
{
struct node *current=head, *temp=current->next;
int a;
while(current!=NULL&&temp!=NULL)
{
a=temp->data;
temp->data=current->data;
current->data=a;
temp=temp->next;
current=current->next;
}
}
