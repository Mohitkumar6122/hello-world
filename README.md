# hello-world
#pragma GCC optimize ("O3")
// #pragma GCC target ("sse4")

// #include <bits/stdc++.h>

// using namespace std;
// typedef long long ll;
// typedef long double ld;
// typedef complex<ld> cd;

// typedef pair<int, int> pi;
// typedef pair<ll,ll> pl;
// typedef pair<ld,ld> pd;


// #define ff(i, a, b) for ( int i=a; i<(b); i++)
// #define ffr(i, a) for (int i=0; i<(a); i++)
// #define fd(i,a,b) for (int i = (b)-1; i >= a; i--)
// #define ffd(i,a) for (int i = (a)-1; i >= 0; i--)
// #define endl "\n"
// #define sz(x) (int)(x).size()
// #define mp make_pair
// #define pb push_back
// #define f first
// #define s second
// #define lb lower_bound
// #define ub upper_bound
// #define all(x) x.begin(), x.end()



// const int mod = 1000000007;
// const ll INF = 1e18;
// const int MX = 2000000001; //check the limits, dummy	 

// int binary_search(int a[],int l,int r,int x){
   
//  if (r>=l){
//     int m=(l+(r-1))/2;
//     if (a[m]==x) { 
//                     return m;
//                  } 
//     else if (a[m]<x)  binary_search(a,m+1,r,x);
//     else    binary_search(a,l,m-1,x);
//   }
  
//   cout<<"ELEMENT NOT FOUND\n";
//   return -1;
// }
   
// void bubble_sort_recursive(int a[],int n){
//   if (n==1) 
//      return;
  
//   for(int i=0;i<n-1;i++)
//     if (a[i]>a[i+1])
//       swap(a[i],a[i+1]);

//   bubble_sort_recursive(a,n-1);     
  
// }
// void printArray(int a[], int n) 
// { 
//     for (int i=0; i < n; i++) 
//         printf("%d ", a[i]); 
//     printf("\n"); 
// }
// class node{
//   public:
//   int data;
//   node* next;

// };

// void fib(int n) 
// { 
//   /* Declare an array to store Fibonacci numbers. */
//   int f[n+2];   // 1 extra to handle case, n = 0 
//   int i; 
  
//   /* 0th and 1st number of the series are 0 and 1*/
//   f[0] = 0; 
//   f[1] = 1; 
  
//   for (i = 2; i <= n; i++) 
//   { 
//       /* Add the previous 2 numbers in the series 
//          and store it */
//       f[i] = f[i-1] + f[i-2]; 
//   } 
  
//   cout<<f[n]<<" "; 
// } 
// class dnode{
//   public:
//   int data;
//   node*next;
//   node*prev;
// };
// // void pushd(node**head,int x){
// //   dnode* nwn=new node();
// //   nwn->data=x;
// //   nwn->next=(*head);
// //   nwn->prev=NULL;
// //   (*head)->prev=nwn;
// //   (*head)->next=nwn;
// // }
// // void delete_dnode(node**head,node*del){
// //   if (*head==NULL|| del==NULL) return;
// //   if (*head==del){
// //     *head=del->next;
// //   }
// //   if (del->next!=NULL)
// //   del->next->prev=del->prev;
// //   if(del->prev!=NULL)
// //   del->prev->next=del->prev;
  
// //   free(del);
// //   return ;
// // }
// void bub_sort_linked(node* head){
//   node*cur=head,*ind;
//   int temp;
//   if (head==NULL) return;
//   else{
//     while(cur!=NULL){
//      ind=cur->next;
//       while(ind!=NULL){
//         if (cur->data>ind->data){
//           temp=cur->data;
//           cur->data=ind->data;
//           ind->data=temp;
//         }
//         ind=ind->next;
//    } cur=cur->next;

//   }
//   }
// }
// void print_linked_list(node*n){
//   int i=1;
//   while(n!=NULL){
//     cout<<n->data<<" ";
     
//     n=n->next; 
//     i++;
//   }
//  cout<<"\n";  //cout<<"NOT PRESENT IN LINKED LIST \n";

// }
// void insert(node* n,int x){
//   node*new_node=new node();
//   new_node->data=x;
//   new_node->next=n->next;
//   n->next=new_node;
//   }
// void sorted_insert(node**n,int x){
//   node* c;
//   node* new_node=new node();
//   new_node->data=x;
//   if(*n==NULL||(*n)->data>=x){
//     new_node->next=*n;
//     *n=new_node;
//   }
//   else{
//     c=*n;
//     while(c->next!=NULL && c->data<x){
//       c=c->next;
//     }
//     new_node->next=c->next;
//     c->next=new_node;
//   }
// }
// void delete_node(node** n ,int x){
//   node*temp=*n;
//   node* prev;
//   if (temp!=  NULL &&temp->data==x){
//     *n=temp->next;
//     free(temp);
//     return;
//   }

//   while(temp!=NULL &&temp->data!=x){
//     prev=temp;
//     temp=temp->next;
//   }
//   if (temp==NULL) return;

//   prev->next=temp->next;
//   free(temp);
// }

// void skipMdeleteN(node *head,int M ,int N){
//   node *curr=head,*t;
//   int count;
//   while (curr)
//  { for(int count=1;count<M && curr!=NULL;count++){
//       curr= curr->next;
//   }
//   if (curr==NULL)
//   return;
//  t=curr->next;
//   for(int count=1;count<=N && t!=NULL;count++){
//     node*temp=t;
//     t=t->next;
//     free(temp);
//   }
//   curr->next=t;
//   curr=t;
// }
// }

// bool palindrome(node *head){
//    node* temp=head;
//   stack<int>s;
//   while(temp!=NULL){
//     s.push(temp->data);
//     temp=temp->next;
//   }
//   while(head!=NULL){
//     int i=s.top();
//     s.pop();
//     if (head->data!=i) {return false;
//   }
//   head=head->next;
//   }
//   return true;
//   }

// void traverse_Cirular_linkd(node*head){
//   node*temp=head;
//   if( head!=NULL){
//     do{
//       cout<<temp->data;
//      temp=temp->next;
//     }
//     while(temp!=head);
//   }
// }
// void delfn(node**head,int n){
//   int count;
//   node*curr=*head;
//   for(count=1;count<=n&&curr!=NULL;count++){
//     node * t=curr;
//     curr=curr->next;
//     free(t);
//   }
//   *head=curr;
// }
// void show_stack(stack<int> stck){
//   while(!stck.empty()){
//     cout<< stck.top()<< " ";
//     stck.pop();
//   }
// }

// vector < ll > v[100000];
// vector < ll > visited  ;

// ll c, z, i, q, k, m, x,  b, n, t,  ans =0, res = 0;
// string str , str2 ;
// char chr ;

// int  dfs( int s ){ //cout << s<< endl ;
  
//   visited [s] = 1 ;
//   //cout << s << endl; 
//   for(int i = 0;i < v[s].size(); i++){
//      if (v[s][i] == k ) { 
//            cout << "YES" << endl ;
//           exit(0);
//         }  
//     if (!visited[v[s][i]] ){
//      // cout << v[s][i] << endl ;
//       dfs(v[s][i]);
//     }
//   }
//  cout << "NO" ;
//  exit(0) ;

// }

// ll a[100000] ;
// class tree{
//   public :
//   int data ;
//   tree* left ;
//   tree* right ;
// }
// int main()
//  {
// 	ios_base::sync_with_stdio(0) ,cin.tie(0);
    
//   //   int a[]={8,5,3,11,44,56,2,6,3444,23,56,94,3342,35} ;
//   //   n=sizeof(a)/sizeof(a[0]);
   
//   //   node*head;
//   //   node* sec;
//   //   node* th;
//   //   head=new node();
//   //   sec=new node();
//   //   th=new node();
//   //   head->data=1;
//   //   head->next=sec;
//   //   sec->data=2;
//   //   sec->next=th;
//   //   th->data=3;
//   //   th->next=NULL;
//   //   print_linked_list(head);
//   //   insert(head->next->next,5);
//   //   print_linked_list(head);
//   //   sorted_insert(&head,8);
//   //   sorted_insert(&head,23);
//   //   sorted_insert(&head,2);
//   //   sorted_insert(&head,3);
//   //   sorted_insert(&head,0);
//   //   sorted_insert(&head,9);
//   //   sorted_insert(&head,86);
//   //   sorted_insert(&head,33);
//   //   sorted_insert(&head,19);
//   //   print_linked_list(head);
//   //   delete_node(&head,67);
//   //   delete_node(&head,3);
//   //   print_linked_list(head);
//   //   skipMdeleteN(head,2,2);
//   //   print_linked_list(head);
//   // if (palindrome(head))cout<<"PALINDROME\n";
//   // else
//   // cout<<"NOT A PALINDROME\n";
//   //  bub_sort_linked(head);
//   //  print_linked_list(head);
   

//   //   stack<int> st;
//   //   st.push(4);
//   //   st.push(5);
//   //   st.push(5);
//   //   st.push(6);
//   //   st.push(7);
//   //   st.push(8);
//   //   show_stack(st);
//   // int rr=4;
//   // int ff=34;
//   //   int ask=fib(rr);
//   //   int asd =fib(ff);
//   //   cout<<ask<<" "<<asd;
//   // ll nodes, edges, y ;
//   // cin >> nodes >> k ;
//   // ff(i,1,nodes + 1 ){
//   //     visited.push_back(0);
//   //   }

//   //  ff(i,1,nodes ) cin >> a[i] ; 
  
//   // for(int i=1; i < nodes  ; i++){
//   //      v[i].push_back(a[i] + i) ;
//   //     //cout << i << a[i] + i << endl ;
//   // }
//   //  (dfs(1)) ;
//   cin >> t ;
//   while (t--) {
//   vector< pair <ll, ll> > score ;
//   cin >> n ;
//   ff(i, 0, n) cin >> a >> b, score.pb(mp(a, b)) ;
//   ll pl = score[0].f, cl = score[0].s ;
//   ff(i, 1, n) {
//     if ( (score[i].s > cl && score[i].f <= pl) || score[i].s < cl) { cout << "NO\n" ; break;}
//     else if (score[i].s == cl && score[i].f < pl){cout << "NO\n" ; break;}
//     else if ( i == n - 1) cout <<"YES\n" ; 
//     else pl = score[i].f, cl = score[i].s ;
//   }
//   }
// }


// cin >> n >> x ;
//   ll money[n] ;
//   ff(i, 0, n) cin >> a, money[i] = a - x ;
//   sort(money, money + n) ;
//   temp = 0, ans = 0 ;
//   fr(i, 0, n) {
//     if (temp + money[i] >= 0) ans++, temp += money[i] ;
//     else break ;
//   }
//   cout << ans << endl  ;
//   }
// }

//   while(t--) {
//     cin >> x >> n >> m ;
//     res = n ;
//     while (res != 0){
//       if ( x <= 20) break ;
//       x = ( x / 2) + 10 ;
//       res-- ;
      
//     }
//     if ( x - m * 10 <= 0) cout << "YES\n" ;
//     else cout <<"NO\n" ;
//   }
// }

//     cin >> n ;
//     temp = 3, res = 2 ;
//     while ( n % temp != 0) {
//       temp += pow(2, res) ;
//       res++ ;
//     }
//     cout << n /temp << endl ;
//   }
// }

// cin >> n ;
//     temp = 0, res = -1 ;
//     if ( (n / 2) & 1) cout <<"NO\n" ;
//     else { cout <<"YES\n" ;
//       ff(i, 0, n / 2) temp += 2, cout << temp << " " ;
//       ff(i, 0, n / 2 - 1) res += 2, cout << res  << " " ;
//       cout << n + (n /2 - 1) << endl ;
//     }
//   }
// }

//  cin >> n ;
//     ll a[n] ;
//     ff(i, 0, n) cin >> a[i] ;
//     ll temp = a[0], sum = 0  ;
//     ff(i, 1, n ) {
//       if (a[i] * temp > 0){
//         if ( temp < a[i] ) { temp = a[i] ; continue ;}
//       }
//       else sum += temp, temp = a[i] ;
//     }
//     cout << sum + temp << endl ;
//   }
// }

//  cin >> n >> k ;
//     ll a[n] ;
//     temp = 0, res = -INF, ans = 0 ;
//     ff(i, 0, n) cin >> a[i] ;
//     map < ll, ll > ma ;
//     ff(i, 0, n / 2){
//       temp = a[i] + a[ n - i - 1] ;
//       ma[temp]++ ;
//     }
//     temp = 0 ;
//     for ( auto x : ma) {
//       if ( x.s > temp) res = x.f, temp = x.s ;
//     }
//     ff(i, 0, n / 2) {
//       if (a[i] + a [n - i - 1] != res){
//         if ( res - max(a[i], a[n - i - 1]) > k) ans += 2 ;
//         else ans++ ;
//       }
//     }
//     cout << ans << endl ;
//   }
// }
// cin >> t ;
// while(t--) {
//     ll d ; temp = res = x = y = 0 ;
//     cin >> n >> a >> b >> c >> d ;
//     temp = abs( a - b) * n ;
//     res = (a + b) * n ;
    
//     if ( temp >= c + d ||res <= c - d ))cout <<"No\n" ;
//     else cout <<"Yes\n" ;
//   }
// }   


//  while(t--) {
//     cin >> x >> y >>a >> b ;
//     cout << max(0ll, min((x + y)*a, ((min(x,y) * b)+ abs(x - y) * a))) ;
//     cout << endl ;
//   }
// }

// while(t--) {
//     cin >> n ;
//     cout << pow(2, (1 + n/2)) - 2 << endl ;
//   }
// }


//  sort(s.begin(), s.end());
 
//     if (s[0]!=s[k-1])
//     {
//         cout<<s[k-1]<<endl;
//         return;
//     }
//     bool eq = true;
//     for (int i = k; i+1<s.size(); i++) if (s[i]!=s[i+1]) eq = false;
//     if (!eq) cout<<s[0] + s.substr(k)<<endl;
//     else {
//         string ans;
//         for (int i = 0; i<s.size(); i+=k) ans+=s[i];
//         cout<<ans<<endl;
//     }


//  while(t--) {
//     cin >> n >> k ;
//     set < ll > sa ;
//     vector < ll>  v(n), aa ;
//     ff(i, 0, n) cin >> v[i], sa.insert(v[i]) ;
//     sort(all(v)) ;
//     temp = v[n - 1] ;
//     if ( sa.size() > k) cout << -1<< endl  ;
//     else { 
//       ff(i, 0, max(temp, k)) aa.pb(1 + i ) ;
//       cout << n * n<< endl ;
//       ff(i, 0, n*n) {
//         cout << aa[i % aa.size()] << " " ;
//       }cout << endl ; 
//     }sa.clear() ;
//   }
// }    

