let NFTs = [];

function mintNFT(_name, _facecolor, _pantType, _bling) {
    const NFT = {
        "name": _name,
        "facecolor": _facecolor,
        "panttype": _pantType,
        "bling": _bling
    };
    NFTs.push(NFT);
    console.log("Minted: " + _name);
}

function listNFTs() {
    for (let a = 0; a < NFTs.length; a++) {
        console.log(`Name: ${NFTs[a].name}`);
        console.log(`Face Color: ${NFTs[a].facecolor}`);
        console.log(`pant Type: ${NFTs[a].panttype}`);
        console.log(`Bling: ${NFTs[a].bling}`);
        console.log("\n");
    }
}

function getTotalSupply() {
    console.log("Total Number of NFTs: " + NFTs.length);
}

// Call your functions below this line
mintNFT("ghanshyam", "black", "full pant", "diamond chain");
listNFTs();
getTotalSupply();
