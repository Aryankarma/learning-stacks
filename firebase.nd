    // get single document from a collection
    const uid = auth.currentUser?.uid;

    // const docRef = doc(db, uid, "docID1");
    // const docData = await getDoc(docRef);

    // if (docData.exists()) {
    //   console.log(docData.data())
    // } else {
    //   console.log("could not fetch document");
    // }

    // get multiple documents from a collection or subCollection
    // const queryToGetMultipleDocuments = query(collection(db, uid), where('field1', "==", "value1"))
    // const docData = await getDocs(queryToGetMultipleDocuments);

    // get all documents in a collection
    let tempDatesData: String[] = [];

    const queryToGetAllDatesData = await getDocs(collection(db, `${uid}/`));

    queryToGetAllDatesData.forEach((input) => {
      tempDatesData = [...tempDatesData, input.id];
    });

    // const queryToGetAllSessionData = await getDocs(
    //   collection(db, `${uid}/${tempDatesData[0]}/session`)
    // );

    // queryToGetAllSessionData.forEach((input) => {
    //   tempSessionData = [...tempSessionData, input.id];
    // });

    // const getDataFromDate1Session1 = await getDoc(
    //   doc(db, uid, "28 July 2024", "session", "session21:26")
    // );

