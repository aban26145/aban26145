const sha256 =require('sha256');
function Blockchain (){
      this.chain=[];
this.createNewBlock(100,'500','100');
}
Blockchain.prototype.creatNewBlock=function(nonce,            prevBlockhash,hash){
     const newBlock ={
       index:this.chain.length+1,
       timestamp: this.pendingTransaction,
       nonce:nonce,
       prevBlockhash: prevBlockhash,
       hash:hash,
  };
this.pendingTransaction=[];
this.chain.push(newBlock);
        return newBlock;
}
             
